# My Data Science Portfolio 🚀

Hi, I'm Eren. Since my recent work in the fashion retail industry contains proprietary data and trade secrets (NDA), I cannot share the raw source code here. 

However, I wanted to share the **architecture, tools, and logic** behind the systems I built.

Here is a breakdown of what I've been working on:

## 1. Automated Product Tagging (Computer Vision)
At my previous job, we needed to tag thousands of product photos with attributes like "Color" and "Pattern" automatically. Manual tagging was too slow.

* **My Approach:** I built a hybrid pipeline.
* **Tools I Used:**
    * **YOLO & DINOv2:** To detect where the clothing item is in the image.
    * **SAM (Segment Anything Model):** To cut out the specific cloth from the background cleanly.
    * **K-Means Clustering:** To mathematically find the dominant colors (RGB) and map them to our color catalog.
* **Result:** We automated the catalog data entry process significantly.

## 2. SQL Query Optimization
Some of our daily operational reports were taking too long to run, causing timeouts on the server.

* **What I Did:** I analyzed the execution plans of legacy T-SQL procedures. I realized they were using inefficient cursors and missing indexes.
* **The Fix:** I rewrote the logic using proper JOINs and optimized the indexes based on query patterns.
* **Result:** Execution times dropped by about **60%**, making the reports instant.

## 3. Recommendation Engine
To increase cross-sales, I designed a system to suggest items that go well together (e.g., "People who bought this shirt also bought these pants").

* **The Logic:** I used the **Apriori Algorithm** to analyze past transaction data and find strong association rules between products.
* **Integration:** I wrote SQL procedures to serve these recommendations directly to the front-end applications.

*Feel free to reach out via [LinkedIn](https://www.linkedin.com/in/eren-baykara-534110228) if you want to discuss the technical details!*
