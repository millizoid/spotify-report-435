# Spotify Songs Project

## Abstract

In this study, we conducted an in-depth analysis of Spotify song data to unveil the intricate relationships between various predictor variables and the response variable, popularity. It takes the results from analyzing the popularity of the top songs on Spotify in the years 2021 and 2022 and dives into what other variables influence song popularity. Leveraging a generalized linear model (GLM) with an extensive array of interactions, we systematically examined the significance of factors such as explicitness, release year, artist prominence, acoustic characteristics, song length, and energy levels. Our results, as determined through ANOVA and Wald tests, illuminated the nuanced impact of these variables and their interactions on song popularity. Noteworthy main effects were identified, including the substantial influence of the release year, explicit content, and top artist prominence. Furthermore, significant interaction effects, such as the interplay between year and top artist status, underscored the complexity of factors contributing to song popularity. These findings were visually represented through bar plots, providing a comprehensive overview of estimated coefficients and their confidence intervals, enhancing our understanding of the intricate dynamics shaping musical preferences on the Spotify platform. This research contributes valuable insights into the multifaceted nature of song popularity, offering a foundation for further exploration and refinement of predictive models in the evolving landscape of music consumption.

## Introduction

In this study, I extend my exploration of the dynamic realm of popular
music by conducting a comprehensive analysis to identify the factors
that significantly contribute to a song's popularity in the years 2021
and 2022. Building upon previous research that examined the distinctions
between these two pivotal years, the focus shifts towards fitting the
best model using Generalized Linear Modeling (GLM) and Logistic
Regression to discern the key determinants of high popularity scores.
For more information on the previous research, refer to Project 1
@R-Project1.

The variables under scrutiny encompass explicit content, principal
artist followers, acousticness, year, song length, and energy, all of
which are posited as potential significant factors influencing a song's
popularity on Spotify. This investigation seeks to unravel the nuanced
interplay of these variables and their collective impact on the evolving
landscape of popular music.

Unlike the earlier exploration, which primarily aimed at discerning
differences between the years 2021 and 2022, this research aims to
provide a more nuanced understanding by delving into the specific
factors that contribute to elevated popularity scores. The Spotify
popularity metric remains the linchpin of our assessment, offering a
standardized measure to gauge the songs' relative popularity.

Through a meticulous application of statistical methodologies, this
study aims to uncover insights that transcend mere temporal comparisons.
Rather than focusing on year-to-year disparities, the analysis strives
to pinpoint the underlying factors that consistently drive heightened
popularity across both 2021 and 2022.

As I look into this data, I anticipate that explicit content, principal
artist followers, acousticness, year, song length, and energy
collectively weave a complex narrative that shapes the success of songs
in the Spotify ecosystem. This nuanced perspective aims to move beyond
the binary contrast of years and shed light on the multifaceted
influences that contribute to a song's enduring appeal.

The outcomes of this research will not only enrich our understanding of
the intricate fabric of popular music but also serve as a valuable
resource for artists, industry professionals, and music enthusiasts. By
unraveling the nuanced determinants of song popularity, this study aims
to provide actionable insights that contribute to the continuous
evolution of the music landscape.

Null:
$H_{0}^{2}: \beta_{Explicit} = \beta_{Year} = \beta_{Acousticness} = \beta_{Energy} = \beta_{Song Length} = \beta_{Artist Followers} = 0$

This means none of the examined variables have a significant impact on
the popularity of songs.

Alternative: At least one of the coefficients
($\beta_{Explicit}, \beta_{Year}, \beta_{Acousticness}, \beta_{Energy}, \beta_{Song Length}, \beta_{Artist Followers}$)
$\neq0$
