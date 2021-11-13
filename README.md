# logging

Simple logging functionality with Tensorboard and SQLite for ML training. Combines the functionality of Tensorboard and SQLite to have more capabilities in analysing ML experiments.

# Functionality

Start an experiment. The experiment will get unique name given all the parameters previously added to the logger. Based on this it is possible to later reload each specific ML model setup for testing etc., if all relevant parameters are added here. See [LegalSum](https://github.com/sebimo/LegalSum) for examples for model loading (LegalSum/src/model.py: parse_run_parameters, reload_model).

All added performance metrics will be tracked in every epoch and stored in SQLite + visualized in Tensorboard. The addition of SQLite allows easier analysis/access, if the Tensorboard visualization and data is not enough.

# Usage
See __main__ part in logger.py
