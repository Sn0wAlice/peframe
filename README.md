# peframe

**peframe** is an open-source tool to perform static analysis on **Portable Executable (PE)** malware and generic suspicious files.

It helps malware researchers detect:

- Packers  
- XOR-encoded strings  
- Digital signatures  
- Mutex  
- Anti-debugging techniques  
- Anti–virtual machine techniques  
- Suspicious sections and functions  
- Macros  
- And much more  

---

## Install

### Download

```bash
sudo apt install git
git clone https://github.com/guelfoweb/peframe.git
cd peframe
```

### Installation script for Ubuntu

```bash
sudo bash install.sh
```

### Installation (prerequisites required)

```bash
sudo python3 setup.py install
```

---

## Prerequisites

The following dependencies are required before installing and using **peframe**:

```text
python >= 3.6.6
python3-pip
libssl-dev
swig
```

---

## Usage

```bash
peframe -h
```

Examples:

```bash
peframe filename            # Short output analysis
peframe -i filename         # Interactive mode
peframe -j filename         # Full output analysis (JSON)
peframe -x STRING filename  # Search XORed string
peframe -s filename         # Strings output
```

### Note

You can edit the `config-peframe.json` file located in the `config/` folder to configure your VirusTotal API key.

After installation, use:

```bash
peframe -h
```

to find the API configuration path.

---

## How it works

### MS Office (macro) document analysis – peframe 6.0.1

[![MS Office analysis](https://asciinema.org/a/mbLd5dChz9iI8eOY15fC2423X.svg)](https://asciinema.org/a/mbLd5dChz9iI8eOY15fC2423X?autoplay=1)

### PE file analysis – peframe 6.0.1

[![PE analysis](https://asciinema.org/a/P6ANqp0bHV0nFsuJDuqD7WQD7.svg)](https://asciinema.org/a/P6ANqp0bHV0nFsuJDuqD7WQD7?autoplay=1)

---

## Talk about...

- [A Longitudinal Analysis of Brazilian Financial Malware](https://www.lasca.ic.unicamp.br/paulo/papers/2020-TOPS-marcus.botacin-brazilian.bankers.pdf)  
  *(Federal University of Paraná, Marcus Botacin et al., 2020)*

- [Building a smart and automated tool for packed malware detections using machine learning](https://dial.uclouvain.be/memoire/ucl/en/object/thesis%3A25193)  
  *(Université catholique de Louvain, Minet & Roussieau, 2020)*

- [Revealing Packed Malware](https://www.researchgate.net/publication/220496734_Revealing_Packed_Malware)  
  *(NJIT, Nirwan Ansari)*

- [Critical Infrastructures Security: Improving Defense Against Novel Malware and APTs](https://iris.uniroma1.it/retrieve/handle/11573/1362189/1359415/Tesi_dottorato_Laurenza.pdf)

- [Anatomy on Malware Distribution Networks](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9057639)

- [Intel Owl 0.4.0](https://github.com/certego/IntelOwl/releases/tag/0.4.0)

- [Machine Learning Aided Static Malware Analysis: A Survey and Tutorial](https://www.researchgate.net/publication/324702503_Machine_Learning_Aided_Static_Malware_Analysis_A_Survey_and_Tutorial)

- [SANS DFIR Poster 2016](http://digital-forensics.sans.org/media/Poster_SIFT_REMnux_2016_FINAL.pdf)

- [Suspicious File Analysis with PEframe](https://eforensicsmag.com/download/malware-analysis/)

- [CERT-FR Security Bulletin](https://www.cert.ssi.gouv.fr/actualite/CERTFR-2014-ACT-030/)

---

## Other

This tool is currently maintained by **Snow Alice**  
But originally developed by **Gianluca Guelfo** (guelfoweb).
https://github.com/guelfoweb/peframe

Suggestions and criticism are welcome.