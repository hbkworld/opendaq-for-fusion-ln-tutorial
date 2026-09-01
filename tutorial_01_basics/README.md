# Tutorial 01: Connecting to Fusion LN via openDAQ

This tutorial is a single Jupyter notebook, [tutorial_01.ipynb](tutorial_01.ipynb), that walks through using openDAQ's Python bindings to connect to and work with a single Fusion LN module.

## What it covers

- Creating an openDAQ Instance and adding a custom function block module path
- Discovering and connecting to a Fusion LN device
- Configuring channels: sensor type (IEPE/Voltage), sampling rate, activating/deactivating channels, TEDS, high-pass filter, input range
- Reading sample-aligned data with a `MultiReader` and plotting it
- Scaling raw signals to engineering units (via sensor sensitivity) and visualizing with a Renderer function block
- Saving data to WAV, binary UFF, and CSV files, and validating each against the original data

## Prerequisites

- Python 3.9+
- A Fusion LN device reachable on your network
- Jupyter (e.g. `pip install notebook`, or use VS Code's Jupyter extension)
- Create and activate a virtual environment, then install dependencies into it:

  ```bash
  python -m venv .venv

  # Windows
  .venv\Scripts\activate

  # macOS/Linux
  source .venv/bin/activate

  pip install -r requirements.txt
  ```

  > Keeping dependencies in a virtual environment avoids version conflicts with other Python projects on your machine. If using VS Code or Jupyter, select the `.venv` interpreter/kernel before running the notebook.

## Running

Open [tutorial_01.ipynb](tutorial_01.ipynb) in Jupyter or VS Code and run the cells in order. Update the connection string in the "Adding FusionLN" cell to match your device.

## Note

The tutorial was tested with the Fusion LN firmware ver. 3.3.0.1362 and 3.5.0.2545. In the future firmware releases, the sensitivity of TEDS-enabled sensors will be supported by the firmware. In the referenced versions, it is not; therefore a special attention is paid to getting the sensitivity values/units from the TEDS and applying it.

