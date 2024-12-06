# Template Board Design for 340

## General Information

Here everything you need to know:

- The completed board design is ready to go - `template_inverting.zip` is ready to be uploaded to JLC as-is.
- If you want to inspect the board design in Altium or make changes, this repo is also the Altium project itself. Open `Lab_M3.PrjPcb` to view it.
- There are several reference images and utilities contain in `media/`.

## Build Notes

All the components have their values printed on the board, and those values were chosen based on the inventory of the shop at the time. If the shop inventory were to change significantly, you might have to do some rework by replacing footprints (though most parts likely still fit). For now though, the only thing that is not a one to one component match from the LTSpice design is that the shop did not have 100nF capacitors, so we used a 90nF and a 10nF in parallel.

## Parts List

| **Component**    | **Quantity** | **Notes**                                                          |
|------------------|--------------|--------------------------------------------------------------------|
| **Capacitors**   |              |                                                                    |
| 1mF              | x2           | mult. colors in the shop, green and black have the best tolerance. |
| 1uF              | x1           |                                                                    |
| 90nF             | x4           | 1/2 of the 100nF setup.                                            |
| 10nF             | x4           | 1/2 of the 100nF setup.                                            |
| 50pF             | 2            | The shop has 56pF, which is close enough.                          |
| **Resistors**    |              |                                                                    |
| 200k             | x2           |                                                                    |
| 2.5k             | x1           | The shop has 2.4k, which is close enough.                          |
| 1k               | x4           |                                                                    |
| 330              | x1           |                                                                    |
| 100              | x2           |                                                                    |
| 6                | x1           | can be made with mult. or use a power resistor                     |
| **Misc**         |              |                                                                    |
| MCP6002          | x1           | Part of the kit                                                    |
| 2106A            | x1           | Part of the kit                                                    |
| LED              | x1           | Part of the kit                                                    |
| Photodiode       | x1           | Part of the kit                                                    |
| 4-pin header (F) | x1           |                                                                    |
| 2-pin jumper     | x1           |                                                                    |
| 1-pin TP         | x2           |                                                                    |

## Reference Images

![Image of the board design](/images/board_design.png)

![Image of the board design](/images/drc_summary.png)

![Image of the board design](/images/schematic_altium.png)

![Image of the board design](/images/fft_ltspice.png)