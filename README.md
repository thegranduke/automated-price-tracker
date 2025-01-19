# Automated Price Tracking Tool

Welcome to the Automated Price Tracking Tool! This Python-based application empowers you to monitor product prices across various e-commerce platforms effortlessly. By leveraging web scraping and automation, it ensures you stay informed about price fluctuations, helping you make cost-effective purchasing decisions.

---

## Features

- **User-Friendly Interface:** A minimalist UI built with Streamlit allows you to add or remove products from your tracking list seamlessly.
- **Comprehensive Dashboard:** Visualize price history for each tracked product, enabling easy monitoring of trends.
- **Customizable Alerts:** Set price drop thresholds and receive instant notifications via Discord when prices fall below your specified percentage.
- **Automated Scheduling:** The tool updates product prices at intervals you define, ensuring you have the latest information without manual checks.
- **Scalable Architecture:** Designed to work with any e-commerce website, providing flexibility in your price tracking endeavors.

---

## Prerequisites

Before you begin, ensure you have the following:

- **Python 3.8+** installed on your system.
- **Virtual Environment:** Set up a virtual environment to manage dependencies.
- **Discord Account:** For receiving price drop notifications.
- **GitHub Account:** To host the application and utilize GitHub Actions for scheduling.
- **Supabase Account:** For hosting a free PostgreSQL database instance.

---

## Installation

1. **Clone the Repository:**
    
    ```
    git clone https://github.com/your-username/automated-price-tracking-tool.git
    cd automated-price-tracking-tool
    ```
    
2. **Set Up Virtual Environment:**
    
    ```
    python -m venv .venv
    source .venv/bin/activate  # On Windows, use `.venv\Scripts\activate`
    ```
    
3. **Install Dependencies:**
    
    ```
    pip install -r requirements.txt
    ```
    
4. **Configure Environment Variables:**
    
    Create a `.env` file to store your configuration details, such as Discord webhook URL and Supabase credentials.
    

---

## Usage

1. **Run the Application:**
    
    ```
    streamlit run ui.py
    ```
    
2. **Add Products:**
    
    Use the sidebar to input product URLs you wish to track.
    
3. **Set Price Drop Thresholds:**
    
    Define the percentage drop at which you want to be notified.
    
4. **Receive Notifications:**
    
    When a product's price drops below your specified threshold, you'll receive an alert via Discord.
    

---

## Scheduling Price Checks

To automate price checks, utilize GitHub Actions to run the application at defined intervals. This setup ensures your price data is always up-to-date without manual intervention.
