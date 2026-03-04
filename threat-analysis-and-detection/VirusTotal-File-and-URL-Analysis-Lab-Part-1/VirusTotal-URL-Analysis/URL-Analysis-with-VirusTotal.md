# URL Analysis with VirusTotal

## Objective
Given a scenario, analyze potential indicators to determine the type of attack.

## Description
VirusTotal is a free online service that analyzes files and URLs to identify potential malware. It combines 70 antivirus scanners and URL/domain blacklisting services along with other tools to identify malware.

---

## Steps

### 1. Navigate to VirusTotal
Returned to the VirusTotal home page using the browser's back button after completing the file scan.

- Navigated to [**`virustotal.com`**](https://www.virustotal.com/gui/home/upload)
- Clicked the **URL** tab

![SS11](/threat-analysis-and-detection/VirusTotal-File-and-URL-Analysis-Lab-Part-1/Screenshots/SS11.png)

### 2. Enter the URL
Entered the school's URL (**`https://www.citytech.cuny.edu/`**) into the search field and clicked **Search**.


### 3. Wait for Analysis to Complete
Waited for VirusTotal to finish scanning the URL across all security vendors.

### 4. Review Details Tab

![SS13](/threat-analysis-and-detection/VirusTotal-File-and-URL-Analysis-Lab-Part-1/Screenshots/SS13.png)

**Result:** 0 / 94 security vendors flagged the URL as malicious.
 
### 5. Review Detection Tab
Clicked the **DETECTION** tab to view individual vendor results.

![SS12](/threat-analysis-and-detection/VirusTotal-File-and-URL-Analysis-Lab-Part-1/Screenshots/SS12.png)

**Notable result:** ESET flagged the URL as **Suspicious**, while the majority of vendors returned **Clean**.

### 6. Review Vendor Analysis, Unrated Sites
Scrolled through the full list of vendor analysis results.

**Finding:** Approximately 30% of vendors returned **Unrated** for this URL, meaning they had no data on it.

![SS14](/threat-analysis-and-detection/VirusTotal-File-and-URL-Analysis-Lab-Part-1/Screenshots/SS14.png)

---


## Key Findings

- The URL **`https://www.citytech.cuny.edu/`** was flagged as clean by the vast majority of the 94 vendors polled.
- About **30% of vendors returned Unrated**, meaning they simply don't have the site in their database yet, this does not indicate malicious activity.
- Multiple vendors correctly categorized the site as an **educational institution**, confirming it is a known, legitimate domain.
