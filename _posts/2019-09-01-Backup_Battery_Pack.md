---
layout: post
title:  Backup Battery Pack
date:   2019-09-01 08:00:00 +0530
image:  2019-Backup-Battery-Pack/img_01.jpg
---
In this project, I've built a Li-ion battery pack that is capable of charging directly from a solar panel. The battery pack has `75` cells in a `3`-cell configuration which results in a `12V` output. I used an external inverter to convert the DC output of the battery to `230VAC`.

![]({{ site.baseurl }} /media/2019-Backup-Battery-Pack/img_05.jpg)
*Battery pack with the external inverter*

Since I had planned on charging the battery using a solar panel, I used a Maximum Power Point Tracking (`MPPT`) module. The maximum charging current of this unit is `5A`. A Battery Management System (`BMS`) oversees the charging and discharging cycles of the battery and, it is capable of a maximum current draw of 100A.

![]({{ site.baseurl }} /media/2019-Backup-Battery-Pack/img_06.jpg)
*Spot Welded battery pack*

I arranged the batteries in a `3`-cell series and `25`-cell parallel(3s25p) configurations to get a 12V output. The cells were spot-welded using the [Spot welder](https://lkbrilliant.github.io/2019/07/12/Spot_Welder), which I built during my last project. You can find more information about the Spot Welded on its [project page](https://lkbrilliant.github.io/2019/07/12/Spot_Welder). The `12V` output of the battery can be connected to an inverter to convert the DC voltage into mains AC voltage. The following diagram shows the interconnections of the components in the system.

![]({{ site.baseurl }} /media/2019-Backup-Battery-Pack/model_02.png)
*CAD drawing of the enclosure*

I used Fusion360 to design the enclosure. When making the enclosure, first, I designed all the parts inside the CAD program and logically arranged them. After doing that, I designed the enclosure around it. Placing the parts beforehand allowed me to optimize the component placement in a tight space.

![]({{ site.baseurl }} /media/2019-Backup-Battery-Pack/img_03.jpg)
*Internal view of the battery pack*

![]({{ site.baseurl }} /media/2019-Backup-Battery-Pack/model_01.png)
*All the parts were arranged before designing the enclosure*

Due to the limited space, steady airflow is critical for cooling the modules during operation, hence the 6mm cooling fan on the top.

![]({{ site.baseurl }} /media/2019-Backup-Battery-Pack/img_02.jpg)
*Parts I used for this project*

I used the following parts and components to build this project.

- 1 x `18V` Solar Panel: `100W`
- 1 × Solar MPPT Charge Controller: `BQ24650`
- 1 × Li-ion Battery Management System: Maximum discharge current `100A`
- 1 × Digital Voltmeter / Ammeter Panel: `0-100VDC / 0-10A`
- 75 × `18650` Li-ion cell: `3.7V`
- 2 × `XT90` connectors
- 1 × Inverter: `12VDC-230VAC 1000W`
- 1 × Cooling fan: `12V-6x6mm`

![]({{ site.baseurl }} /media/2019-Backup-Battery-Pack/img_07.jpg)
*Interconnections of the components*

## Design Files

You can find all the CAD files of this project on my [GitHub](https://github.com/LKbrilliant/Backup-Battery-Pack) page.