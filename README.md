# SSH Brute-Force Attack Pattern Analysis

## 1. Ask the Question (Step 1)
**Question:** Based on public honeypot data, which geographic regions and specific password patterns are most commonly used in automated SSH brute-force attacks?
**Benefit:** This analysis helps in understanding global threat landscapes and prioritizing security measures like Geo-blocking or Fail2Ban configurations for organizations worldwide.

## 2. Determine the Data Needed (Step 2)
For this project, I am using publicly available **Open Data** instead of private logs:
* **Honeypot SSH Logs:** Datasets from sources like **Kaggle** (e.g., "SSH Honeypot Logs") or the **Dshield** project.
* **IP-to-Country Mapping:** Databases for converting IP addresses into geographic locations.
* **Common Password Lists:** Reference lists (like RockYou) to compare with the passwords used by attackers in the logs.

## 3. Methodology & Tools
* **Type of Analysis:** Descriptive Analysis (historical data patterns).
* **Language:** Python 3.x
* **Libraries:** `pandas` for data manipulation, `matplotlib/seaborn` for generating heatmaps of attacks.

## 4. Hypothesis
I hypothesize that a significant portion of automated traffic originates from cloud-hosting provider regions and that the vast majority of attacks attempt to gain access using the 'root' username and common default passwords.
