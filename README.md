# OpenMC Crash Course

A hands-on introduction to Monte Carlo neutron transport with OpenMC. You’ll build and run a pin-cell model, then use what you’ve learned to visualize reactor geometry, score tallies, and work through a depletion example for a molten chloride fast reactor (MCFR).

The course is designed for five 90-minute sessions, split between instruction and hands-on practice. Some familiarity with Python and the command line will help. If you’re new to OpenMC, start with Week 0 (installation).

## Getting started

Clone the repository and open the course folder in your terminal.

```bash
git clone https://github.com/williamhm412/crash_course_openmc.git
cd crash_course_openmc
```

Follow the Week 1 slides to set up OpenMC and the nuclear data used in the course. The Windows instructions use Ubuntu through WSL. For Linux and macOS setup, see the [OpenMC installation guide](https://docs.openmc.org/en/stable/usersguide/install.html).

Once OpenMC is installed, use the [post-install guide](https://github.com/williamhm412/crash_course_openmc/blob/main/week1/run_after_install_guide.md) to open a notebook in Jupyter or VS Code.

## Course outline

| Week | Topic | Slides | Hands-on work |
| --- | --- | --- | --- |
| 0 | Course orientation | [Introduction](https://github.com/williamhm412/crash_course_openmc/blob/main/week0/week0_intro.pptx) | See what OpenMC can do and how the course is organized. |
| 1 | Install and verify OpenMC | [Installation](https://github.com/williamhm412/crash_course_openmc/blob/main/week1/week1_install.pptx) | Set up your Python environment, configure nuclear data, and verify that OpenMC runs. |
| 2 | Model components and particle transport | [Background](https://github.com/williamhm412/crash_course_openmc/blob/main/week2/week2_background.pptx) | Practice defining materials, surfaces, cells, boundary conditions, and sources in the [workbook](https://github.com/williamhm412/crash_course_openmc/blob/main/week2/week2_workbook.ipynb). For extra practice, try the [pin-cell walkthrough](https://github.com/williamhm412/crash_course_openmc/blob/main/week2/pincell/pincell.ipynb) or run the [Python example](https://github.com/williamhm412/crash_course_openmc/blob/main/week2/pincell/pincell.py). |
| 3 | Cross sections and your first complete model | [OpenMC basics](https://github.com/williamhm412/crash_course_openmc/blob/main/week3/week3_basics.pptx) | Use the [workbook](https://github.com/williamhm412/crash_course_openmc/blob/main/week3/week3_workbook.ipynb) to learn how to set up a run. Build a pin cell from the [starter notebook](https://github.com/williamhm412/crash_course_openmc/blob/main/week3/pincell_empty/pincell_empty.ipynb), then compare your work with the [completed example](https://github.com/williamhm412/crash_course_openmc/blob/main/week3/pincell_completed/pincell_completed.ipynb). |
| 4 | Reactor geometry and visualization | [Advanced modeling](https://github.com/williamhm412/crash_course_openmc/blob/main/week4/week4_advanced.pptx) | Follow the [MCFR-D walkthrough](https://github.com/williamhm412/crash_course_openmc/blob/main/week4/mcfr_D/mcfr_D.ipynb), then build and visualize your own [MCFR-C model](https://github.com/williamhm412/crash_course_openmc/blob/main/week4/mcfr_C/mcfr_C.ipynb) using the [reference workbook](https://github.com/williamhm412/crash_course_openmc/blob/main/week4/mcfr.xlsx). |
| 5 | Tallies, depletion, and parallel computing | [Final session](https://github.com/williamhm412/crash_course_openmc/blob/main/week5/week5_final.pptx) | Work through tallies and depletion in the [MCFR-D notebook](https://github.com/williamhm412/crash_course_openmc/blob/main/week5/MCFR_D/mcfr_D.ipynb), then [extend your MCFR-C model](https://github.com/williamhm412/crash_course_openmc/blob/main/week5/MCFR_C/readme.md) from Week 4. |

For the full list of theory and skills covered each week, see the [course overview](https://github.com/williamhm412/crash_course_openmc/blob/main/course_overview.pdf).

## References

- The pin-cell examples draw on the [OpenMC pin-cell tutorial](https://github.com/openmc-dev/openmc-notebooks/blob/main/pincell.ipynb).
- The MCFR exercises use representative models from TerraPower’s [*Representative Neutronics Models of MCFR Reactors*, Rev. 0 (2023)](https://github.com/williamhm412/crash_course_openmc/blob/main/week4/MCFR-ENG-PRSNT-0021Rev0-1.pdf).
- For help with OpenMC syntax and model setup, see the [OpenMC User’s Guide](https://docs.openmc.org/en/stable/usersguide/index.html).

Feel free to share the course with anyone learning OpenMC. If you have questions or feedback, email [williamhm412@gmail.com](mailto:williamhm412@gmail.com).
