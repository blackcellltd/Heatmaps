# Heatmaps
Sector specific MITRE ATT&CK heatmaps for detection engineering 

Introduction

Black Cell strives to always be one step ahead of cyber criminals, which means we must always stay up to date on the threats that target our customers. However, our customers come in all shapes and sizes, therefore the adversaries that target one customer will likely use very different techniques than those who target another. In order to provide accurate and tailored recommendations, it is not enough to audit your infrastructure; we must also look towards other organizations within your market sector. In parallel with the infrastructure assessment, we have analysed the most notable threats that have led to the successful compromise of other organizations in your sector. We have collected, analysed, and mapped the TTPs used in these attacks to the MITRE ATT&CK framework in order to provide a heatmap of which techniques pose the greatest threat to your organization.

Sector Specific Analysis of Adversary TTPs

The usefulness of threat intelligence can be measured in its ability to deny cyber-attacks when adequate mitigations are in place. An excellent illustration of this concept is David Bianco’s Pyramid of Pain.  This simple diagram shows the relationship between the types of indicators we might use to detect an adversary's activities and how much effort or “pain” it will cause them when you are able to deny them the use of those indicators.When we are able to detect and mitigate TTPs, we are covering entire adversary behaviours, not just their tools. From a pure effectiveness standpoint, this is ideal. If we are able to prevent or react to adversary TTPs in a timely fashion, we can force them to do the most time-consuming thing possible, learn new behaviours. Therefore, with the results of this assessment in combination with the analysis of sector specific TTPs, you will receive actionable intelligence about where to focus your efforts, in order to cause as much possible headache for would-be attackers. 

Methodology

There are numerous sources of historical data and high-quality analyses of cyber threats that can be used to map out sector specific TTPs. Therefore, out analysis starts with the aggregation of appropriate data in terms of quantity and quality from a range of sources. Our data gathering starts with a search of the clear web, which is essentially everything that is indexed by the most popular search engines. For our research we used Google Dork because it strongly supports targeted OSINT work. Dorking (or Google Hacking) is a technique used by security researchers that utilizes specialized queries written in Google’s own query language, to find highly specialized resources. For further data enrichment we used a deep web metasearch engine, called SearX. Where applicable we also used cyber-attack information from Cyber Intel Matrix, which is a CTI platform that crawls TOR, I2P and Zeronet/Freenet sources among others.
After having identified the most substantial incidents (and threats), we used the previously described data collection methodologies to determine the specific approaches and procedures that led to the successful cyber-attack. Mapping these procedures to ATT&CK techniques is trivial and is sometimes even included in publicly available analyses. We also collected any available signatures to identify the malwares and tools that were used. Many of these tools could be directly searched in the MITRE ATT&CK resources to determine exactly what techniques they enable.

It is also not uncommon to find threat actors that operate exclusively in a given sector. It is therefore worthwhile identifying the APT groups or other criminal gangs behind the cyber-attacks under review, in order to identify trends in the methods they employ. This threat profile may contain exploitation tools, malwares, and typical techniques that they have used in previous attacks. 
Finally, it is also necessary to review the security gaps that victimized the affected entity. Often times searches for such information will not be fruitful, however when this information can be gathered, it is incredibly useful. The security gaps and inadequacies that resulted in successful cyber-attacks, serve as excellent points of reflection, allowing us to consider how these gaps apply to our own environments and enable us to learn from others’ mistakes.
In summary our data collection process can be broken down into the following steps.

  Find the most relevant cyber incidents and threats.
  
  Gather all available information about the incidents.
    Pinpoint the tools or malwares that were used.
    Determine attack procedures and methodologies that were used.
    Map this information to ATT&CK techniques. 
  
  Identify the threat actors (APT, criminal groups) and build a threat profile.
    Collect information about their tools and attack procedures.
    Map this information to ATT&CK techniques. 
  
  Determine the inadequacies of the victim. 
    Map these security gaps to ATT&CK techniques. 

Not all the information collected is of equal value. Some attack information is more impactful, and others are less relevant. Therefore, it is important to quantify the collected information in a from that can be further analysed. Part of this process is simply the mapping of attack information to ATT&CK techniques; however, we also need to assign some sort of a numerical score to each cyber threat. 
As such, the following scoring system was devised. Each cyber threat was given an impact score in the range of 1-5. A score of 1 indicates the incident could be resolved in a matter of days. A score of 3 indicates that substantial and lasting damage was sustained by the victim. A score of 5 indicates a substantial risk to human life or lasting societal damage. 

The threats were also given an evasion score in a range of 1-5. A score of 1 indicates the threats could have been detected by relatively simplistic signature-based detections tools, whilst a score of 5 indicates that highly sophisticated detection evasion methods were used.

A similar complexity score was also assigned to each threat, that indicates the competence, experience, and knowledge level of the adversary. A score of 1 indicates the adversary is only capable of using existing tools (colloquially a “script kiddie”), whilst a score of 5 means the adversary is capable of writing custom tailored malware. 

Another important score is the proven historical successfulness of the threat. A score of 1 indicates no or partial success, while 5 indicates perfect execution and complete success in achieving its goals. 

Finally, due to the volume of the data and the diversity of data sources, we also assign an accuracy multiplier, that reflects our certainty and confidence in our findings. The final scores are then mapped to ATT&CK techniques and normalised to a scale of 1-7 (1 being critical severity threats and 7 being low severity threats), before being displayed on the heatmap.
