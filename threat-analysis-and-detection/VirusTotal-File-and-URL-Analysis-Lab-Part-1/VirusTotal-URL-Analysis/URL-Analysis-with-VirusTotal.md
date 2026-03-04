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

![SS13](/threat-analysis-and-detection/VirusTotal-File-and-URL-Analysis-Lab-Part-1/Screenshots/SS13.png)

**Result:** 0 / 94 security vendors flagged the URL as malicious.

![SS12](/threat-analysis-and-detection/VirusTotal-File-and-URL-Analysis-Lab-Part-1/Screenshots/SS12.png)
  
### 4. Review Detection Tab
Clicked the **DETECTION** tab to view individual vendor results.

**Notable result:** ESET flagged the URL as **Suspicious**, while the majority of vendors returned **Clean**.
