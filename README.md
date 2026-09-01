# openDAQ for Fusion LN Tutorials

A collection of independent, self-contained tutorials for working with HBK Fusion LN via [openDAQ](https://opendaq.com/). Each tutorial lives in its own folder and can be followed on its own — no need to complete them in order.

## Tutorials

| # | Tutorial | Language | Description |
|---|----------|----------|-------------|
| 01 | [tutorial_01_basics](tutorial_01_basics) | Python | Connect to a single Fusion LN module via openDAQ and perform basic operations: setting channel sampling rate, applying a high-pass filter, activating channels, and more. |

## Prerequisites

Each tutorial folder lists its own specific prerequisites in its `README.md`. 

## Repository structure

```
tutorials/
├── README.md              <- this file, index of all tutorials
├── LICENSE
├── CONTRIBUTING.md
├── .gitignore
└── tutorial_01_basics/     <- one self-contained tutorial per folder
    ├── README.md
    ├── requirements.txt
    └── tutorial_01.ipynb
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for how to add a new tutorial.

## License

This repository is licensed under the [MIT License](LICENSE).
