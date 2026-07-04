# R Code for PartLength Comparison: Machine 1 vs. Machine 2

library(ggplot2)
library(plotly)

df_machine_1_2 <- subset(X028...028, Machine == 1 | Machine == 2)

# Independent Samples t-test
t_test_result <- t.test(PartLength ~ Machine, data = df_machine_1_2)
# --- T-Test Results ---

	Welch Two Sample t-test

data:  PartLength by Machine
t = -25.609, df = 2317.9, p-value < 2.2e-16
alternative hypothesis: true difference in means between group 1 and group 2 is not equal to 0
95 percent confidence interval:
 -0.9883242 -0.8477276
sample estimates:
mean in group 1 mean in group 2 
       48.72696        49.64498 

# --- End T-Test Results ---

p_boxplot <- ggplot(df_machine_1_2, aes(x=as.factor(Machine), y=PartLength, fill=as.factor(Machine))) +
    geom_boxplot(alpha=0.7) +
    labs(
        title="PartLength Comparison: Machine 1 vs. Machine 2",
        x="Machine",
        y="PartLength"
    ) +
    scale_fill_manual(values=c("#0072B2", "#D55E00")) +
    theme_minimal() +
    theme(
        axis.title = element_text(size=18),
        axis.text = element_text(size=14),
        legend.position = "none",
        panel.background = element_rect(fill = "white", colour = NA),
        plot.background = element_rect(fill = "white", colour = NA)
    )

p_boxplot_plotly <- ggplotly(p_boxplot)
htmlwidgets::saveWidget(p_boxplot_plotly, "media/plots/machine_1_2_partlength_boxplot.html", selfcontained = TRUE)

