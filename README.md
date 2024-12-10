# AAAI-2024

# Project Title

**Benchmarking of Time Series Foundation Models for Energy Load Forecasting of Commercial and Residential Buildings**


## Description

* In this paper, we present a benchmark study of four state-of-the-art pre-trained Time Series Foundational Models(TSFM), Lag-Llama, TimesFM, Moirai and Chronos aiming to evaluate their performance for short-term load forecasting with diiferent baseline models.

* This repository contains code to load pre-trained models and run predictions.

## Installation

''To replicate the zero-shot experiment setup used in the paper, please follow these steps:''

* Step 1: Create separate environments for each model since they have different dependencies.
* Step 2: Follow the instructions in the readme file given in models' repository to install and setup.
          [TimesFM](https://github.com/google-research/timesfm),
          [Lag-Llama](https://github.com/time-series-foundation-models/lag-llama),
          [Chronos](https://github.com/amazon-science/chronos-forecasting),
          [Moirai](https://github.com/SalesforceAIResearch/uni2ts),
          [TFS](https://nixtlaverse.nixtla.io/neuralforecast/docs/getting-started/introduction.html),
          [Auto-ARIMA](https://auto.gluon.ai/stable/index.html),
          [LightGBM, Linear Regression](https://skforecast.org/0.14.0/index.html).
* Important: You'll need at least 16GB RAM to run TimesFM.

## Results

<table>
    <tr>
        <td>Dataset</td>
        <td colspan="4">TSFM</td>
        <td colspan="2">TFS</td>
        <td colspan="3">Traditional ML Models</td>
    </tr>
    <tr>
        <td></td>
        <td>Chronos</td>
        <td>Lag-Llama</td>
        <td>Moirai</td>
        <td>TimesFM</td>
        <td>Patch-TST</td>
        <td>TFT</td>
        <td>LightGBM</td>
        <td>Linear Regression</td>
        <td>Auto-ARIMA</td>
    </tr>
    <tr>
        <td>Enernoc</td>
        <td>21.37</td>
        <td>38.34</td>
        <td>30.29</td>
        <td>23.44</td>
        <td>28.71</td>
        <td>37.14</td>
        <td>25.64</td>
        <td>26.06</td>
        <td>43.70</td>
    </tr>
    <tr>
        <td>IBlend</td>
        <td>25.46</td>
        <td>37.17</td>
        <td>50.12</td>
        <td>30.98</td>
        <td>37.13</td>
        <td>40.72</td>
        <td>29.52</td>
        <td>30.86</td>
        <td>49.56</td>
    </tr>
    <tr>
        <td><b>Average</b></td>
        <td><b>23.42</b></td>
        <td>37.76</td>
        <td>40.21</td>
        <td><i>27.21</i></td>
        <td>32.92</td>
        <td>38.93</td>
        <td>27.53</td>
        <td>28.46</td>
        <td>46.63</td>
    </tr>
    <tr><td></td></tr>
    <tr>
        <td>CEEW</td>
        <td>105.43</td>
        <td>111.71</td>
        <td>147.59</td>
        <td>98.35</td>
        <td>97.07</td>
        <td>104.17</td>
        <td>113.60</td>
        <td>107.56</td>
        <td>108.07</td>
    </tr>
    <tr>
        <td>Ireland</td>
        <td>101.71</td>
        <td>109.33</td>
        <td>93.79</td>
        <td>88.76</td>
        <td>95.84</td>
        <td>97.96</td>
        <td>106.05</td>
        <td>110.53</td>
        <td>110.17</td>
    </tr>
    <tr>
        <td>MFRED</td>
        <td>24.52</td>
        <td>61.05</td>
        <td>26.33</td>
        <td>25.14</td>
        <td>29.19</td>
        <td>33.90</td>
        <td>33.29</td>
        <td>34.68</td>
        <td>41.48</td>
    </tr>
    <tr>
        <td>NEEA</td>
        <td>86.66</td>
        <td>98.30</td>
        <td>83.40</td>
        <td>80.07</td>
        <td>78.29</td>
        <td>88.94</td>
        <td>90.13</td>
        <td>92.49</td>
        <td>86.66</td>
    </tr>
    <tr>
        <td>NEST</td>
        <td>71.33</td>
        <td>85.15</td>
        <td>72.16</td>
        <td>65.67</td>
        <td>72.01</td>
        <td>69.64</td>
        <td>68.88</td>
        <td>71.13</td>
        <td>75.62</td>
    </tr>
    <tr>
        <td>Prayas</td>
        <td>112.40</td>
        <td>125.57</td>
        <td>165.17</td>
        <td>94.27</td>
        <td>92.41</td>
        <td>113.63</td>
        <td>89.10</td>
        <td>89.21</td>
        <td>126.30</td>
    </tr>
    <tr>
        <td>SMART*</td>
        <td>69.01</td>
        <td>86.63</td>
        <td>65.37</td>
        <td>61.91</td>
        <td>71.13</td>
        <td>68.59</td>
        <td>102.14</td>
        <td>106.14</td>
        <td>71.83</td>
    </tr>
    <tr>
        <td><b>Average</b></td>
        <td>81.58</td>
        <td>96.82</td>
        <td>93.40</td>
        <td><b>73.45</b></td>
        <td><i>76.56</i></td>
        <td>82.40</td>
        <td>86.17</td>
        <td>87.39</td>
        <td>88.59</td>
    </tr>
</table>
