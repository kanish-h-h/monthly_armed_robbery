# Time Series Analysis of Monthly Robberies in Boston (1966-1974)

## Project Overview

This project focuses on analyzing the monthly robbery incidents in Boston from 1966 to 1974 using a manually configured ARIMA model. The aim is to identify patterns and make future predictions based on historical data. 
The project model is saved at `models/`. 

## Dataset

The dataset consists of monthly records of robbery incidents in Boston between 1966 and 1974. The data is sourced from ![](https://github.com/kanish-h-h/monthly_armed_robbery/blob/main/data/Robberies.csv) and is stored in the file `data/Robberies.csv`.

## Project Structure

The project is organized into the following directories and files:

```
.pickle_files/
    
data/ 
    nb_data/
        
    Robberies.csv
        
    armed_robberies.zip
        
images/
    
model/
    
notebook/
	
README.md
```

## Installation

Clone the repository:

```shell
git clone https://github.com/kanish-h-h/monthly_armed_robbery.git
cd monthly_armed_robbery
```

## Pickle file

**model.pkl** can be found at folder `.pickle_files/` for storing the model as pkl.

## Usage

1. **Data Preparation:** Start by running the `Armed_Robberies_in_Boston.ipynb` notebook to clean and prepare the dataset and converts those into `datasets.csv`, `validation.csv` and `stationary.csv`. 
2. **ARIMA Modeling:** Use the `Armed_Robberies_in_Boston.ipynb` notebook to configure and train the ARIMA model on the prepared data over  manually configured.
3. **Fine Tuning**: Fine tuning is done via Grid Search method for finding the optimal `p`, `d` and `q`, for the ARIMA.

## Results

The results of the analysis, including time series plots and ARIMA model diagnostics, are saved in the `images/` directory.

![](https://github.com/kanish-h-h/monthly_armed_robbery/blob/main/images/dataset_plot_kde_hist.png)

![](https://github.com/kanish-h-h/monthly_armed_robbery/blob/main/images/acf_and_pacf.png)

Result on validation dataset
![](https://github.com/kanish-h-h/monthly_armed_robbery/blob/main/images/result_on_validation_data.png)


Time Series Plot
![](https://github.com/kanish-h-h/monthly_armed_robbery/blob/main/images/box_and_whisker_plot.png)

![](https://github.com/kanish-h-h/monthly_armed_robbery/blob/main/images/box_cox_transformed.png)

Residual Error
![](https://github.com/kanish-h-h/monthly_armed_robbery/blob/main/images/residual_error_for_ARIMA.png)

![](https://github.com/kanish-h-h/monthly_armed_robbery/blob/main/images/acf_and_pacf_residual_error.png)


## Conclusion

The ARIMA model provides a robust framework for analyzing and predicting time series data. This project demonstrates how to manually configure and apply an ARIMA model to real-world data, yielding insights into the patterns of robbery incidents in Boston over the observed period.
