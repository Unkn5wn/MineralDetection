# MineralDetection
A mineral detection game
# Report: Challenges in AI-Based Automated Water/Land Detection from Uploaded Maps

**Date:** 2026-03-15  
**Prepared by:** Project Team

---

## 1. Introduction

This project set out to develop an interactive educational game centered on the Strait of Hormuz, requiring users to identify and act only within water zones on a map image. The initiative aimed to rely on artificial intelligence (AI) and related technologies to automatically distinguish and restrict actions to water areas on any uploaded map.

---

## 2. Objectives

- Enable users to interactively select only “water” areas on arbitrary map images.
- Use artificial intelligence or automation to parse water/land boundaries without manual intervention.
- Validate the efficacy of automated boundary detection in a browser-based educational context.

---

## 3. Findings

- **Current AI Limitations:**  
  Existing AI models and browser tools **cannot reliably extract water/land boundaries** purely from uploaded bitmap images without external data or manual annotation.
  
- **Manual Intervention Required:**  
  For this project, water boundaries had to be manually traced—despite AI prompting—using either coordinate arrays or annotated reference images.
  
- **Susceptibility to Error:**  
  Manual estimation, even when guided by tools or overlays, can lead to inaccuracies. Edge cases, irregular coastlines, and islands may be marked incorrectly.
  
- **Integration Challenges:**  
  Pixel-based semantic segmentation (where each image pixel is classified as land or water using AI) is not standard in typical web programming or AI APIs, and not readily accessible to most developers or educators for arbitrary maps.

---

## 4. Scenario and Proof-of-Concept

This project successfully demonstrated a **proof-of-concept**: it is possible to restrict user actions to hand-annotated “water” areas using polygons and coordinate arrays. However, the process highlighted present-day weaknesses in fully automated, AI-driven map understanding.

---

## 5. Conclusion

Artificial intelligence has made significant progress, but **is not yet capable of seamlessly and accurately distinguishing water from land on arbitrary, uploaded static map images without help**. Errors may occur in boundary detection, impacting user experience. As such, **manual steps or semi-automated approaches remain necessary** for real-time or web-based interactive applications that depend on accurate geographic awareness.

---

## 6. Recommendations

- Incorporate a **human-in-the-loop** approach or use pre-existing segmented (e.g., vector, GeoJSON) data for any critical or production applications.
- Monitor developments in AI-based semantic segmentation and consider integration as tools become more mature and accessible.
- Consider combining AI predictions with user guidance for improved accuracy.

## 7. Resources 
If you would like access to the map that I used here is the link and a shout out: https://www.freeworldmaps.net/ocean/hormuz-strait/
---

**End of Report**
