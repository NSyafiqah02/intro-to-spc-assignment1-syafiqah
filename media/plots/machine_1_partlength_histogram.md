# R Code for PartLength Histogram - Machine 1

library(ggplot2)
library(plotly)

df_machine <- subset(X028...028, Machine == 1)

p <- ggplot(df_machine, aes(x=PartLength)) +
    geom_histogram(binwidth=0.5, fill="#0072B2", color="white") +
    labs(
        title="PartLength Distribution for Machine 1",
        x="PartLength",
        y="Frequency"
    ) +
    theme_minimal() +
    theme(
        axis.title = element_text(size=18),
        axis.text = element_text(size=14),
        panel.background = element_rect(fill = "white", colour = NA),
        plot.background = element_rect(fill = "white", colour = NA)
    )

p_plotly <- ggplotly(p)
htmlwidgets::saveWidget(p_plotly, "media/plots/machine_1_partlength_histogram.html", selfcontained = TRUE)

