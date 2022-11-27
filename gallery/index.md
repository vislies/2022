---
layout: default
gallery-nav:
  - title: Not to Scale
    url: "#not-to-scale"
  - title: Pancake Success
    url: "#pancake-success"
  - title: Union Pay
    url: "#union-pay"
  - title: A Feast of Pies
    url: "#a-feast-of-pies"
  - title: For Further Reading
    url: "#for-further-reading"
---

# VisLies 2022 Gallery

After two years of having to meet through cameras and screens, we were
finally able to meet in person for VisLies again.

## Not to Scale

<a href="https://drive.google.com/file/d/14bA7RavmTt-cTVNBiPtmyOy0KEb7arBf/view?usp=sharing" class="image-right">
<img src="lie.png" class="lie" style="left:250px;" />
![](human-to-not-scale-thumb.png)
</a>

[Ken Moreland] started out with a fun example from an [amazon.com product
page for carbon filters]. As with most listing, several pictures are
provided for the product. One of the pictures, shown here, is dedicated to
demonstrating the size and provides a silhouette of a person to help with
scale.

At first glance, the filter pads look huge. The pad is nearly half the
height of a person. But wait. If we look at the actual dimensions of the
pad, we see that the pad is only about a foot tall. Either the sizes of the
pad and the person are not to scale, or that person is only a couple of
feet tall.

On top of that, there is a second view of the pad, unfolded this time. The
unfolded pad is labeled at about 4 feet tall. That is clearly not at the
same scale as the folded pad, and also shorter than the average adult.

None of the three items in this picture are to scale with each other, and
human silhouettes are not part of what is being sold. Thus, the only
function the person serves in this picture is to make the product look
larger than it actually is.

[Ken Moreland]: https://www.kennethmoreland.com/
[amazon.com product page for carbon filters]: https://www.amazon.com/Universal-Activated-Replacement-Purifiers-Conditioner/dp/B087M45SL5/ref=sr_1_1

## Pancake Success

<a href="https://drive.google.com/file/d/1d6mJwhbO30xNqjkwxMhctehF9_XMu_N7/view?usp=sharing" class="image-right">
![](pancake-vis-thumb.jpg)
</a>

While visiting a breakfast restaurant, [Ken][Ken Moreland] came across this
compelling advertisement to work there. It features a visualization that
uses two stacks of pancakes to compare an average job with a job at the
restaurant.

Using pancakes as a physical manifestation of a bar chart is not
unreasonable (although the image could be better about getting the size and
orientation of the pancakes more consistent). Of course, the advertisement
is not actually referring to pancakes but rather a notional concept of career
satisfaction. The idea that life success could be quantified in a single
number, particularly when there is no way to know anything about the
reader's career, is comical.

Or maybe the advertisement is talking about physical pancakes. A pancake
restaurant would almost certainly involve more pancakes than his current
job. As compelling as this argument is, [Ken][Ken Moreland] decided to
stick with his current career.

## Union Pay

<a href="https://drive.google.com/file/d/1vgp2LsohBjl05UpdmcP96fFAh7WePlEd/view?usp=share_link" class="image-right">
![](compensation-union-v-nonunion-thumb.jpg)
</a>

[A recent article in Bloomberg Law][Bloomberg article] showed this recent
plot that the title claims suggests "union jobs are taking a back seat."
The plot certainly shows in recent years the non-union pay being larger
than unions, but the claim struck [Ken][Ken Moreland] as a little odd.

The plot itself does not have anything overtly wrong with it. Although the
asymmetric representation of union data (bars) and non-union (line) is a
a bit strange, there is nothing particularly misleading about it. And the
data time range, which goes from present back over 15 years, is not cherry
picked.

<a href="https://news.bloomberglaw.com/daily-labor-report/us-union-jobs-are-taking-back-seat-to-non-union-in-pay-chart" class="image-left">
<img src="lie.png" class="lie" />
![](compensation-union-v-nonunion-title.jpg)
</a>

<div class="image-stop" />

The real problem here is not with the plot itself but with the title. A
common subtle theme at VisLies is using a visualization to draw a
conclusion that is unsupported by the data. In this case, the plot is
showing the _change_ in worker pay, not the total pay. Just because the
white line is over the tan bars, it is not necessarily the case that
non-union workers are paid more than union workers.

[Ken][Ken Moreland] wanted to take a closer look. The [Bloomberg article]
reports that the data comes from the [U.S. Bureau of Labor Statistics].
[Ken][Ken Moreland] pulled the numbers from the same database and [plotted
both the change and total worker pay].

<a href="https://drive.google.com/file/d/12R-GtOIkcno4GCY5YFuhfd_Xzmck1G7d/view?usp=share_link" class="image-full">
![](compensation-union-v-nonunion-total-thumb.jpg)
</a>

The left plot replicates that in the [Bloomberg article]. The right plot
shows the total pay from the same database.[^scale] As we can see in the right
plot, union jobs still, on average, pay more than their non-union
equivalent (for now).

[Bloomberg article]: https://news.bloomberglaw.com/daily-labor-report/us-union-jobs-are-taking-back-seat-to-non-union-in-pay-chart
[U.S. Bureau of Labor Statistics]: https://www.bls.gov/ncs/
[plotted both the change and total worker pay]: compensation-union-v-nonunion.xlsx

[^scale]: We should point out that this plot of total pay has a vertical
    scale that does not go down to zero. This was done to make it easier to
    see the difference between the two line series. But note that, as we
    often criticize during VisLies, this also exaggerates the difference.

## A Feast of Pies

[Pie charts] and related displays are a common theme at VisLies. Apart from
pie charts having some [dubious features], the base metaphor and visual
elements are frequently misused and abused.

<a href="real-pie-chart.jpg" class="image-right">
<img src="lie.png" class="lie" />
![](real-pie-chart-thumb.jpg)
</a>

[Ken Moreland] identified a group of problematic pie charts. The first of
these is this chart presenting the results of a survey of the North
America's favorite pies. The premise of the "real pie chart" that uses
pictures of real pie slices for the wedges of the chart is cute if a little
distracting.

But you might notice that the numbers do not seem to match the proportional
sizes of the slices. For example, the "Apple" slice is labeled "47%", which
should be nearly half the pie. But that is clearly not the case.

The text around the chart explains why this is. The participants of the
study were asked for their _three_ favorite pies. The chart numbers are not
giving the percentage of votes cast, but rather the number of participants
that voted for the pie. Since each person gets 3 votes, the total
percentage of votes adds up to 300%. As the fine print on the bottom says,
the three votes per participants means that the total number of votes adds
up to more than 100%.

Having the pie represent greater than 100% breaks the basic metaphor of the
pie chart, which is showing parts of a whole. A whole is 100%, so showing
the proportion of votes rather than voters would be much less confusing.
But even if we were to accept the concept that the whole is 300%, the chart
is still wrong. The numbers don't add up to 300% either. They add up to
271%. People must have voted for pies that did not make this top ten list.
Not listing the least significant values in a pie chart is common as too
many thin slices can make the chart less readable. But when this is done,
the remaining categories should be grouped into an "other" slice to ensure
that the proportions of the other slices are correct.

<div class="image-stop" />

<a href="degrees-donut.jpg" class="image-right">
<img src="lie.png" class="lie" style="left:225px;" />
![](degrees-donut-thumb.jpg)
</a>

We now take your pie and add a doughnut of nonsense. Here the numbers add up
to 100%, so at least that is good. But, hey, that 1% slice looks awfully
big. And why does 8% take up half of the chart?

So, yeah. None of these slices are proportional to the number. On top of
that, the numbers seem suspect. How is it possible that more people are
getting Master's degrees than Bachelor's degrees? Unfortunately, the
[original post] doesn't put the chart in context, and the labels are not
clear enough.

<div class="image-stop" />

<a href="" class="image-right">
<img src="lie.png" class="lie" style="left:225px;" />
![](bw-donut-thumb.jpg)
</a>

Now we see your doughnut of nonsense and remove the color. The proportions of
these slices are also off. For example, the lower-left slice is clearly
less than 25%.

But now the chart has been poorly copied enough times that the color is
removed and it is impossible to know which number goes with which category.
We also notice that the legend only has 4 categories whereas there are 5
slices. It might be the case that one of the categories got cut off the
picture. In any case, both the color and the cropping would be less of an
issue if the labels were placed with the chart slices themselves rather
than in a separate legend.

[Pie charts]: https://en.wikipedia.org/wiki/Pie_chart
[dubious features]: https://www.perceptualedge.com/articles/visual_business_intelligence/save_the_pies_for_dessert.pdf
[original post]: https://www.reddit.com/r/CrappyDesign/comments/fi0x1t/somewhat_misleading_graph/?utm_source=share&utm_medium=ios_app&utm_name=iossmf
[black and white doughnut]: https://www.reddit.com/r/CrappyDesign/comments/paa5ki/thank_you/?utm_source=share&utm_medium=ios_app&utm_name=iossmf

## For Further Reading

The last couple of years have brought some serious scientific research
relevant to VisLies. The first of these is "[Misinformed by Visualization:
What Do We Learn From Misinformative Visualizations?]" by Lo, Gupta,
Shigyo, Wu, Bertini, and Qu. The authors collected a large corpus of
visualizations marked as flawed on social media. They systematically
sampled and reviewed these visualizations and propose a taxonomy to
classify misleading visualizations. In addition to the paper itself, the
authors helpfully make available a [bad vis browser] that readers such as
ourselves can mine for VisLies. They also provide [their whole flawed
visualization corpus] for an even deeper dive.

<a href="https://leoyuholo.com/bad-vis-browser/" class="image-full">
![](misinformed-vis-page.png)
</a>

[Misinformed by Visualization: What Do We Learn From Misinformative Visualizations?]: https://dx.doi.org/10.1111/cgf.14559
[bad vis browser]: https://leoyuholo.com/bad-vis-browser/ 
[their whole flawed visualization corpus]: https://osf.io/wghxd/ 

<a href="https://dx.doi.org/10.1145/3411764.3445211" class="image-right">
![](covid-viral-vis.png)
</a>

Another relevant publication is "[Viral Visualizations: How Coronavirus
Skeptics Use Orthodox Data Practices to Promote Unorthodox Science Online]"
by Lee, Yang, Inchoco, Jones, and Satyanarayan. This paper analyzes
visualizations from twitter feeds in "anti-mask" communities. The paper
finds that, surprisingly, these communities respected and mimicked science
principles while simultaneously rejecting the science community. There was
a strong focus on data access and analysis as well as a promotion of
correct visualization techniques.

At the same time, the forums rejected analysis from experts. This served to
isolate the community from contrary positions and allowed them to ignore or
reject contrary evidence. The end result was many compelling, but
ultimately incorrect, visualizations.

[Viral Visualizations: How Coronavirus Skeptics Use Orthodox Data Practices to Promote Unorthodox Science Online]: https://dx.doi.org/10.1145/3411764.3445211

<div class="image-stop" />

----
