# NVIDIA/DeepSeek Analysis Pipeline - README

## REQUIREMENTS
Python 3.8+ with these packages: `pandas yfinance requests textblob python-pptx matplotlib`. Install with: `pip install pandas yfinance requests textblob python-pptx matplotlib`

## QUICK START
1. Download the script: `curl -o nvidia_analysis.py https://raw.githubusercontent.com/raiberahul/NVIDIA_DeepSeek/blob/main/nvidia_analysis_pipeline.py`  
2. Configure API keys in the script by editing these values:  
   `"gnews_api_key": "your_gnews_key"` (get from gnews.io)  
   `"reddit_client_id": "your_reddit_id"` (from Reddit Developer Portal)  
   `"alpha_vantage_key": "your_av_key"` (from alphavantage.co)  
3. Run the analysis: `python nvidia_analysis.py`

## OUTPUTS
The script will create:  
- `/analysis_output/analysis_report.pptx` (PowerPoint with results)  
- `/analysis_output/processed_data.csv` (cleaned dataset)

## TROUBLESHOOTING
- For API limits: Add `time.sleep(1)` before API calls  
- Missing modules: Run `pip install --force-reinstall pandas yfinance requests textblob python-pptx matplotlib`  
- Date errors: Ensure format is `YYYY-MM-DD` in the script's CONFIG section

## LICENSE
MIT License - Free for academic and commercial use

---

To update: `curl -o nvidia_analysis.py https://raw.githubusercontent.com/raiberahul/NVIDIA_DeepSeek/blob/main/nvidia_analysis_pipeline.py`  
Replace "yourusername/repo" with your actual GitHub path. For support contact: your@email.com
