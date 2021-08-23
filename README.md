# Awesome-KAPE
In line with other Awesome GitHub repos, Awesome-KAPE serves as a curated list of KAPE-related resources, including but not limited to blog posts, videos, and links to relevant GitHub repos. 

## Official KAPE Links
- [Download KAPE](https://www.kroll.com/en/services/cyber-risk/incident-response-litigation-support/kroll-artifact-parser-extractor-kape)
- [KAPE Enterprise License](https://www.kroll.com/en/services/cyber-risk/incident-response-litigation-support/kroll-artifact-parser-extractor-kape/enterprise-license)
  - TL;DR: if you make money off KAPE in a paid engagement, you need a license! Otherwise, it's free for everyone else including but not limited to Law Enforcement, students, researchers, etc
- [KAPE Training](https://www.kroll.com/en/services/cyber-risk/incident-response-litigation-support/kroll-artifact-parser-extractor-kape/training)

## Tool-Related GitHub Repos

### KAPE

- [KapeFiles](https://github.com/EricZimmerman/KapeFiles) - This repository contains all the Targets and Modules utilized by KAPE to collect and process forensic artifacts
- [KapeDocs](https://github.com/EricZimmerman/KapeDocs) - This repository serves as the backend for KAPE's KapeDocs page, linked [here](https://ericzimmerman.github.io/KapeDocs/)

### EZ Tools

The command line versions of [Eric Zimmerman's Tools](https://ericzimmerman.github.io/#!index.md) ship with KAPE, so they are very relevant to KAPE's overall functionality. The following EZ Tools have KAPE Modules written for them and these repos should be monitored for activity given that they will directly influence KAPE output:

  - [AmcacheParser](https://github.com/EricZimmerman/AmcacheParser)
  - [AppCompatCacheParser](https://github.com/EricZimmerman/AppCompatCacheParser)
  - [bstrings](https://github.com/EricZimmerman/bstrings)
  - [EvtxECmd](https://github.com/EricZimmerman/evtx)
    - Namely, [Maps](https://github.com/EricZimmerman/evtx/tree/master/evtx/Maps) where EvtxECmd Maps are located
  - [JLECmd](https://github.com/EricZimmerman/JLECmd)
  - [LECmd](https://github.com/EricZimmerman/LECmd)
  - [MFTECmd](https://github.com/EricZimmerman/MFTECmd)
  - [PECmd](https://github.com/EricZimmerman/PECmd)
  - [RBCmd](https://github.com/EricZimmerman/RBCmd)
  - [RecentFileCacheParser](https://github.com/EricZimmerman/RecentFileCacheParser)
  - [RECmd](https://github.com/EricZimmerman/RECmd)
    - Namely, [BatchExamples](https://github.com/EricZimmerman/RECmd/tree/master/BatchExamples) where Batch Files are located
    - Also, [RegistryPlugins](https://github.com/EricZimmerman/RegistryPlugins) which are used by RECmd (and Registry Explorer) to generate more efficient/actionable output
  - [SQLECmd](https://github.com/EricZimmerman/SQLECmd)
    - Namely, [Maps](https://github.com/EricZimmerman/SQLECmd/tree/master/SQLMap/Maps) where SQLECmd Maps are located
  - [SrumECmd](https://github.com/EricZimmerman/Srum)
  - [SumECmd](https://github.com/EricZimmerman/Sum)
  - [WxTCmd](https://github.com/EricZimmerman/WxTCmd)

## Resources

### Blog Posts/Guides

- [AboutDFIR's KAPE Guide](https://aboutdfir.com/toolsandartifacts/windows/kape/)
- [Exploring KAPE’s Graphical User Interface in v0.8.2.0](https://www.kroll.com/en/insights/publications/cyber/exploring-kapes-graphical-user-interface)

### YouTube Videos

- [A Guide to Eric Zimmerman's command line tools (EZ Tools)](https://youtu.be/GhCZfCzn2l0)
- [Behind The Incident Eric Zimmerman](https://youtu.be/IuiIGzm7k34)
- [Child Exploitation Investigation – Express Analysis with KAPE](https://youtu.be/-Tgc28hHAhw)
- [Conducting Efficient Insider Threat Investigations using KAPE](https://youtu.be/LxjDUMk0w2g)
- [Enabling KAPE at Scale](https://youtu.be/YF-jDoh8BFM)
- [Enhancing Event Log Analysis with EvtxEcmd using KAPE](https://youtu.be/BIkyWexMF0I)
- [Episode 80: Learning about the KAPE tool.](https://youtu.be/TDpAsSnjhBw)
- [Episode 81: Understanding and Using KAPE Target Files](https://youtu.be/DdUqfktcPa4)
- [Episode 82: Understanding and Using KAPE Module Files](https://youtu.be/aT0xy0VvlSQ)
- [Episode 83: Explaining the KAPE GUI Version -Target Side](https://youtu.be/bCSrUOoDXU4)
- [Episode 84: Explaining the KAPE GUI Version - Module Side](https://youtu.be/2cK7SZjQXuY)
- [Episode 85: Running KAPE through the GUI Version](https://youtu.be/a_x0IgTW67o)
- [Episode 86: Reviewing the Output Created by KAPE](https://youtu.be/HqioWJBmeLA)
- [Episode 87: Introducing and Using Timeline Explorer](https://youtu.be/Hy8ZIc86tCo)
- [Episode 88: Comparing EZViewer to Other Free File Viewers](https://youtu.be/r4X5ONbwlSk)
- [Episode 89: Finding Forensic Badness in 3 Minutes or Less](https://youtu.be/V-pBwAGsQvw)
- [Introduction to KAPE](https://youtu.be/L9H1uj2HSb8)
- [KAPE + EZ Tools and Beyond - OSDFCon 2019 - Eric Zimmerman](https://youtu.be/ZCj7cbWwUOs)
- [Triage Collection and Timeline Analysis with KAPE](https://youtu.be/iYyWZSNBNcw)


