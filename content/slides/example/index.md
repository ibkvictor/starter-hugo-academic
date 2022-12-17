---
title: Slides
summary: An introduction to using Wowchemy's Slides feature.
authors: []
tags: []
categories: []
date: "2019-02-05T00:00:00Z"
slides:
  # Choose a theme from https://github.com/hakimel/reveal.js#theming
  theme: black
  # Choose a code highlighting style (if highlighting enabled in `params.toml`)
  #   Light style: github. Dark style: dracula (default).
  highlight_style: dracula
---

<!-- <object data="http://yoursite.com/the.pdf" type="application/pdf" width="700px" height="700px">
    <embed src="http://yoursite.com/the.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="http://yoursite.com/the.pdf">Download PDF</a>.</p>
    </embed>
</object> -->

# Create slides in Markdown with Wowchemy

[Wowchemy](https://wowchemy.com/) | [Documentation](https://owchemy.com/docs/managing-content/#create-slides)

---

![SEM AA6061 + 3 wt % Chitosan](slides/example/slides/2-0.jpg)

---

## Controls

- Next: `Right Arrow` or `Space`
- Previous: `Left Arrow`
- Start: `Home`
- Finish: `End`
- Overview: `Esc`
- Speaker notes: `S`
- Fullscreen: `F`
- Zoom: `Alt + Click`
- [PDF Export](https://github.com/hakimel/reveal.js#pdf-export): `E`

---

## Code Highlighting

Inline code: `variable`

Code block:
```python
porridge = "blueberry"
if porridge == "blueberry":
    print("Eating...")
```

---

## Math

In-line math: $x + y = z$

Block math:

$$
f\left( x \right) = \;\frac{{2\left( {x + 4} \right)\left( {x - 4} \right)}}{{\left( {x + 4} \right)\left( {x + 1} \right)}}
$$

---

## Fragments

Make content appear incrementally

```
{{%/* fragment */%}} One {{%/* /fragment */%}}
{{%/* fragment */%}} **Two** {{%/* /fragment */%}}
{{%/* fragment */%}} Three {{%/* /fragment */%}}
```

Press `Space` to play!

{{% fragment %}} One {{% /fragment %}}
{{% fragment %}} **Two** {{% /fragment %}}
{{% fragment %}} Three {{% /fragment %}}

---

A fragment can accept two optional parameters:

- `class`: use a custom style (requires definition in custom CSS)
- `weight`: sets the order in which a fragment appears

---

## Speaker Notes

Add speaker notes to your presentation

```markdown
{{%/* speaker_note */%}}
- Only the speaker can read these notes
- Press `S` key to view
{{%/* /speaker_note */%}}
```

Press the `S` key to view the speaker notes!

{{< speaker_note >}}
- Only the speaker can read these notes
- Press `S` key to view
{{< /speaker_note >}}

---

## Themes

- black: Black background, white text, blue links (default)
- white: White background, black text, blue links
- league: Gray background, white text, blue links
- beige: Beige background, dark text, brown links
- sky: Blue background, thin dark text, blue links

---

- night: Black background, thick white text, orange links
- serif: Cappuccino background, gray text, brown links
- simple: White background, black text, blue links
- solarized: Cream-colored background, dark green text, blue links

---

{{< slide background-image="/media/boards.jpg" >}}

## Custom Slide

Customize the slide style and background

```markdown
{{</* slide background-image="/media/boards.jpg" */>}}
{{</* slide background-color="#0000FF" */>}}
{{</* slide class="my-style" */>}}
```

---

## Custom CSS Example

Let's make headers navy colored.

Create `assets/css/reveal_custom.css` with:

```css
.reveal section h1,
.reveal section h2,
.reveal section h3 {
  color: navy;
}
```

---

# Questions?

[Ask](https://github.com/wowchemy/wowchemy-hugo-modules/discussions)

[Documentation](https://wowchemy.com/docs/managing-content/#create-slides)



::: frame
:::

# Introduction

::: frame
Introduction

::: block
Motivation Aluminium remains one of the most widely sought out material
for construction, manufacturing and domestic use.
:::

-   Cost

-   Environmental Effects {Rish Husk Ash, $SiO_2$}

-   Improved Performance

    -   Hardness {Turbine Blades}

    -   Tensile Strength {Pistons}

    -   Electric Conductivity {Electric cables}

    -   Thermal Conductivity {Cooking pots}

    -   Corrosion Resistance {Tubing and pipes}
:::

# Current Approach

## Aluminium Alloy \| Synthetic Ceramic Composite

::: frame
Synthetic Ceramic Composites

  Material                    Authors                          Improvements
  --------------------------- -------------------------------- ----------------------------------------------------------------------
  AC-44200 + $Al_{2}O_{3}$    Kurzawa 2018 `\cite`{=latex}     Ballistic resistance by up to 60 % reduction in projectile velocity.
  AA6061 + $TiC$              Kareem 2021 `\cite`{=latex}      improved wear resistance
  AA7072 + $SiC$              `\cite`{=latex}                  increased tensile and hardness
  Aluminium Alloy + $TiC$     Reddy 2018 `\cite`{=latex}       increased compressive strength
  Aluminium Alloy + $ZrB_2$   Sivakumar 2019 `\cite`{=latex}   increased compressive strength and reduced wear volume
:::

## Aluminium Alloy \| Biodegradable reinforcement materials

::: frame
Biodegradable reinforcement materials

  Material                             Authors                                   Improvements
  ------------------------------------ ----------------------------------------- -----------------------------------------
  Al-Matrix + Wood particles           Omoniyi 2021 [@Omoniyi2021Mechanical]     improved UTS and mechanical properties.
  AA2014 + Egg Shells                  Dwivedi 2016[@Dwivedi2016Synthesis]       improved hardness
  Aluminium Alloy + Rish Husk Ash      Singh 2018[@Singh2018Rice]                improved wear resistance
  $Al-4.5 \% Cu$ + Bamboo Leaf Ash     Kumar Biru 2018[@Kumar2018Experimental]   increased yield strength
  A356 + alloy + Breadfruit Seed Ash   Atunaya 2014 [@Atuanya2014]               decreased wear rate
:::

## Aluminium Alloy \| Hybrid Reinforcements

::: frame
Hybrid Reinforcements

  Material                             Authors                             Improvements
  ------------------------------------ ----------------------------------- --------------------------------------------------------
  AA7075 + $B_{4}C$ + $MoS_2$          Liu 2019[@Liu2019]                  decfease abrasive wear and increased tensile strength.
  AA6082 + $Gr$ + $Y_{2}O_{3}$         Kumar 2020 [@Kumar2020Synthesis]    reduced wear rate and friction coefficient
  AA3003 + $CNT$ + $TiC$               Nayim 2020 [@Nayim2020]             increased hardness
  AA6061 + $TiB_{2}$ + $Al_{2}O_{3}$   David 2018 [@DavidRajaSelvam2018]   increased hardness and tensile strength
  AA6061 + $SiC$ + $Al_{2}O_{3}$       Umanath 2014 [@Umanath2014]         increased micro-hardness
:::

# Methodology

## Materials

---
Materials

-   Aluminium Alloy : AA6061

    -   Aluminium 6061 is a magnesium-silicate alloy with minor iron,
        copper, chromium, zinc, tin, and manganese. Silicon and
        magnesium are the primary alloying constituents of aluminium,
        AA 6061. The material is desired for its features, such as high
        strength and weld-ability.

```{=html}
<!-- -->
```
-   Chitosan

    -   It has appealing properties like high thermal conductivity, high
        tensile and hardness strength.

    -   Chitosan possesses bio-genic antibacterial properties.

    -   Sustainable source of reinforcement material gotten from Dried
        Fish Scales.
---

## Fabrication

---
Filtering and Stir-Casting + Thermal treatment

![Powdered Chitosan at 90 $\mu m$ and Fabricated
Composites](image.png){#fig:your-figure width="\\textwidth"}
:::

## Experiments

---
Experiments

-   Electrical Tests

    -   Conductivity

    -   Resistivity

-   Thermal Tests

    -   Thermal Conductivity

-   Mechanical Tests

    -   Hardness

    -   \% Elongation

    -   Tensile Strength

-   Micro-structural Tests

    -   Hardness

    -   X-ray Diffractometer

    -   Scanning Electron Micrography

    -   Energy Dispersion Micrography
---

## Results

### Thermal properties

---
Thermal properties

::: tabular
c\|c Sample &\
AA6061 & 362.97\
AA6061 + 3 wt. % Chitosan & 141.59\
AA6061 + 6 wt. % Chitosan & 189.40\
AA6061 + 9 wt. % Chitosan & 141.59\
AA6061 + 12 wt. % Chitosan & 124.16\
:::
:::

### Mechanical properties

::: frame
Hardness

![Hardness of Fabricated Aluminium Matrix
Composites](hardness_aa6061.jpg){#fig:your-figure width="\\textwidth"}
:::

::: frame
% Elongation

![% Elongation of Fabricated Aluminium Matrix
Composites](elong_aa6061.jpg){#fig:your-figure width="70%"}
:::

::: frame
Tensile Strength

![Tensile Strength of Fabricated Aluminium Matrix
Composites](tensile_aa6061.jpg){#fig:your-figure width="\\textwidth"}
:::

### Micro-structural properties

::: frame
X-ray Diffractogram

![XRD AA6061](xrd_aa6061.jpg){#fig:your-figure width="\\textwidth"}
:::

::: frame
X-ray Diffractogram \| 3 wt % Chitosan

![XRD AA6061 + 3 wt % Chitosan ](xrd_3.jpg){#fig:your-figure
width="\\textwidth"}
:::

::: frame
X-ray Diffractogram \| 6 wt % Chitosan

![XRD AA6061 + 6 wt % Chitosan](xrd_6.jpg){#fig:your-figure
width="\\textwidth"}
:::

::: frame
X-ray Diffractogram \| 9 wt % Chitosan

![XRD AA6061 + 9 wt % Chitosan](xrd_9.jpg){#fig:your-figure
width="\\textwidth"}
:::

::: frame
X-ray Diffractogram \| 12 wt % Chitosan

![XRD AA6061 + 12 wt % Chitosan](xrd_12.jpg){#fig:your-figure
width="\\textwidth"}
:::

::: frame
Scanning Electron Microscope

![SEM AA6061](image015.jpg){#fig:your-figure width="\\textwidth"}
:::

::: frame
Scanning Electron Microscope \| 3 wt % Chitosan

![SEM AA6061 + 3 wt % Chitosan](image016.jpg){#fig:your-figure
width="\\textwidth"}
:::

::: frame
Scanning Electron Microscope \| 6 wt % Chitosan

![SEM AA6061 + 6 wt % Chitosan](image017.jpg){#fig:your-figure
width="\\textwidth"}
:::

::: frame
Scanning Electron Microscope \| 9 wt % Chitosan

![SEM AA6061 + 9 wt % Chitosan](image018.jpg){#fig:your-figure
width="\\textwidth"}
:::

::: frame
Scanning Electron Microscope \| 12 wt % Chitosan

![SEM AA6061 + 12 wt % Chitosan](image019.jpg){#fig:your-figure
width="\\textwidth"}
:::

### Electrical properties

::: frame
Conductivity

::: columns
::: tabular
c\|c\|c\|c Specimen & Voltage (V) & Current (A) & Conductivity (S/m)\
AA6061 & 0.5 & 1.19 & 37.81\
& 0.5 & 1.14 & 36.21\
& 0.5 & 1.15 & 36.61\
& 0.5 & 1.12 & 35.49\
& 0.5 & 1.20 & 38.20\
:::
:::
:::

# Conclusions

::: frame
Conclusions

-   Hardness of the developed composites improved with higher
    concentration of chitosan particulate; 9 wt.% chitosan reinforced
    sample developed a substantial 4.88 % improvement.

-   The electrical conductivity of aluminium matrix composite reinforced
    with chitosan was reduced compared to unreinforced AA6061 because of
    the introduction of insulation from chitosan reinforcement

-   The synthesized composites showed enhanced tensile strength
    performance with a 25.8 % increase observed the 12 wt.

-   Stir casted AA6061/chitosan provided reduced conductive heat
    transfer coefficient compared to as-cast AA 6061
:::

## Closing Remark

::: frame
Appreciation

::: center
Thank You for listening
:::
:::

::: frame
::: center
Questions ?
:::
:::

## References

::: frame
References
:::
