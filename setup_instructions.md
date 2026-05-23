# Setup Instructions for MycoFabric Experiments

## Prerequisites

1. Microsoft Fabric trial account (60 days free)
2. Create a Lakehouse named `MycoFabricLakehouse`

## Steps to Run

1. Download `Notebook 1.ipynb` from this repository
2. Upload to your Fabric workspace
3. Open the notebook
4. Run cells in order:
   - First cell: Generates synthetic data
   - Remaining cells: Experiments E1-E5
5. Run `GenerateFigures.ipynb` to create figures

## Notes

- All experiments run on F64 trial capacity
- Total runtime: ~2-3 hours
- Results save to `/lakehouse/default/Files/`
