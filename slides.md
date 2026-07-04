---
title-slide: false
bibliography: references.bib
csl: vancouver.csl
citeproc: true
theme: serif
background-color: "#ffffff"
transition: slide
navigationMode: linear
hash: true
---

:::: {.columns}
::: {.column width="50%"}

## Sample slides
#### PlaceHolderName
#### Universiti Malaysia Perlis
#### [placeholder@email.com](mailto:placeholder@email.com)

<!-- __AUDIO_INTRO_DO_NOT_TOUCH__ -->

:::

::: {.column width="50%"}
![](media/pics/logo1.png)
:::

::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide one
**Key Concepts:**
- Energy conservation per @carnot1824.
- $\Delta U = Q - W$
:::

::: {.column width="50%"}
![](media/pics/sample.png)
:::
::::

---

<span class="slide-title" data-title="My Hidden Slide Name"></span>

![](media/pics/wide.jpeg)

---

:::: {.columns}
::: {.column width="50%"}
### The Master Equation
The fundamental relation of thermodynamics:

$$\Delta U = Q - W$$

The work done $W$ is positive when the system expands against an external pressure.
:::

::: {.column width="50%"}
<video data-src="media/videos/sample.mp4" data-autoplay loop muted width="100%"></video>
:::

::::

---

:::: {.columns}
::: {.column width="50%"}
### Visualizing the Gas Law
**Interactive Model:**

- P, V, and T relationships.
- Use the slider to adjust pressure.
- Observe the phase boundary.
:::

::: {.column width="50%"}
<iframe 
  data-src="media/plots/sample.html" 
  width="100%" 
  height="500px" 
  style="border:none;" 
  scrolling="no">
</iframe>
:::
::::

---

## PartLength Histograms by Machine

:::: {.columns}
::: {.column width="50%"}
### Machine 1 PartLength Distribution
<iframe data-src='media/plots/machine_1_partlength_histogram.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::: {.column width="50%"}
### Machine 2 PartLength Distribution
<iframe data-src='media/plots/machine_2_partlength_histogram.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

:::: {.columns}
::: {.column width="50%"}
### Machine 3 PartLength Distribution
<iframe data-src='media/plots/machine_3_partlength_histogram.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::: {.column width="50%"}

:::
::::

---

## PartLength X-bar Control Charts (Temp=338, Pres=200)

:::: {.columns}
::: {.column width="50%"}
### Machine 1 Control Chart
<iframe data-src='media/plots/machine_1_control_chart_xbar_one.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::: {.column width="50%"}
### Machine 2 Control Chart
<iframe data-src='media/plots/machine_2_control_chart_xbar_one.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

:::: {.columns}
::: {.column width="50%"}
### Machine 3 Control Chart
<iframe data-src='media/plots/machine_3_control_chart_xbar_one.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::: {.column width="50%"}

:::
::::

---

## PartLength Process Capability Analysis (Temp=338, Pres=200)
LSL=45, USL=55

:::: {.columns}
::: {.column width="50%"}
### Machine 1 Capability
<iframe data-src='media/plots/machine_1_capability_analysis.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::: {.column width="50%"}
### Machine 2 Capability
<iframe data-src='media/plots/machine_2_capability_analysis.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

:::: {.columns}
::: {.column width="50%"}
### Machine 3 Capability
<iframe data-src='media/plots/machine_3_capability_analysis.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::: {.column width="50%"}

:::
::::

---

## PartLength Comparison: Machine 1 vs. Machine 2

:::: {.columns}
::: {.column width="50%"}
### T-Test Results and Boxplot
Here's a comparison of 'PartLength' between Machine 1 and Machine 2, visualized with a boxplot, alongside the results of an independent samples t-test to assess for a statistically significant difference.

For full R code and t-test output, refer to `media/plots/machine_1_2_partlength_boxplot.md`
:::
::: {.column width="50%"}
<iframe data-src='media/plots/machine_1_2_partlength_boxplot.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::
