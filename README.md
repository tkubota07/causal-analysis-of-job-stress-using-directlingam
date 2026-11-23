# causal-analysis-of-job-stress-using-directlingam
DirectLiNGAMとPythonを用いた職業性ストレス要因の因果探索

Causal discovery of job stress factors using DirectLiNGAM and Python.

## Overview
本リポジトリは、DirectLiNGAM を用いて職業性ストレス関連要因の因果構造を分析するための Python コードを公開するものです。

主な解析内容
- Shapiro-Wilk正規性検定  
- Spearman順位相関分析  
- DirectLiNGAMによる因果探索  
- Bootstrapによる因果効果の安定性評価(n=1000)  
- 誤差独立性検定
- 因果グラフの可視化

This repository contains Python code for causal analysis of job stress factors using the DirectLiNGAM algorithm.

Main Analyses
- Shapiro-Wilk normality test  
- Spearman rank correlation analysis  
- DirectLiNGAM causal discovery  
- Bootstrap estimation(n=1000)  
- Error independence test  
- Causal graph visualization  

## Requirements
- python 3.12.5  
- numpy  
- pandas  
- matplotlib  
- seaborn  
- scipy  
- lingam

## Installation
リポジトリをクローンし、必要なライブラリをインストールします。

git clone https://github.com/tkubota07/causal-analysis-of-job-stress-using-directlingam.git

cd causal-analysis-of-job-stress-using-directlingam

pip install -r requirements.txt

## Usage
Jupyter Notebookを起動し、job_stress_directlingam.ipynb を開いて、セルを上から順番に実行してください

Launch Jupyter Notebook:

jupyter notebook

Open job_stress_directlingam and run the cells sequentially.

## Data
本研究で使用した調査データは、個人情報保護の観点から公開していません。

入力データは、列に分析変数、行に調査対象者を配置した CSV 形式で準備してください。

The original survey data are not publicly available due to privacy restrictions. 

Input data should be provided as a CSV file with variables in columns and participants in rows.

## Methods
解析手順

- データ読込み  
- Shapiro-Wilk検定による正規性検証  
- Spearman順位相関係数の算出  
- DirectLiNGAMによる因果探索  
- Bootstrapによる因果効果の安定性評価(n=1000)  
- 誤差独立性検定  
- 因果グラフ作成  

Analysis Procedure

- Load the dataset  
- Assess normality using the Shapiro-Wilk test  
- Calculate Spearman's rank correlation coefficients  
- Perform causal discovery using DirectLiNGAM  
- Evaluate the stability of causal effects using bootstrap resampling (n = 1,000)  
- Test the independence of error terms  
- Generate a causal graph  

<img width="1853" height="767" alt="図2" src="https://github.com/user-attachments/assets/52464c53-e0f8-412a-8376-f94cd2dc90d4" />

## Results

- Spearman順位相関行列  
- 推定された因果順序  
- DirectLiNGAMによる因果グラフ  
- 推定された総因果効果  
- Bootstrapによる因果効果の安定性評価結果（n = 1,000） 
- 誤差項の独立性検定結果  

- Spearman correlation matrix  
- Estimated causal ordering  
- Estimated causal graph using DirectLiNGAM  
- Estimated total causal effects  
- Stability assessment of causal effects using bootstrap resampling (n = 1,000)  
- Independence test results for error terms  


## Citation
本コードを利用した場合は、以下を引用してください。

If you use this repository, please cite:

Kubota T. Causal Analysis of Job Stress Using DirectLiNGAM. GitHub Repository. 2026.

## License
This project is licensed under the MIT License.

## Author
Takumi Kubota
