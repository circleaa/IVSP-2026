# Style-Aware Data Augmentation for Deep Learning on Symbolic Music

[![Conference](https://img.shields.io/badge/Conference-IVSP_2026-blue.svg)](https://www.ivsp.net/IVSP2026.html)
[![DOI](https://img.shields.io/badge/DOI-10.1117%2F12.3116024-orange.svg)](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/14268/1426811/Style-aware-data-augmentation-for-deep-learning-on-symbolic-music/10.1117/12.3116024.short?tab=ArticleLink#s2)
[![Paper PDF](https://img.shields.io/badge/Paper-Download_PDF-red.svg)](./StyleAware.pdf)

> 本儲存庫收錄發表於 **The 2026 8th International Conference on Image, Video and Signal Processing (IVSP 2026)** 之研究論文全文與相關成果資料。

---

## Publication Details

* **Title:** Style-Aware Data Augmentation for Deep Learning on Symbolic Music
* **Venue:** The 2026 8th International Conference on Image, Video and Signal Processing (IVSP 2026), Meiji University Surugadai Campus, Tokyo, Japan
* **Authors:** Yung-Chi Tseng, **Yu-Chia Wang (通訊作者 / Corresponding Author)**, Yung-An Chen, Chin-Yun Yang, and Yu-Cheng Lin
* **Grant Support:** 國科會專案補助 (NSTC 114-2637-H-155-001)
* **Publisher:** SPIE Digital Library
* **Official Link:** [https://doi.org/10.1117/12.3116024](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/14268/1426811/Style-aware-data-augmentation-for-deep-learning-on-symbolic-music/10.1117/12.3116024.short?tab=ArticleLink#s2)
* **Full Paper:** [📄 點此檢視 / 下載 PDF (Direct PDF Link)](./StyleAware.pdf)

---

## Abstract

在針對特定領域之符號音樂進行深度學習生成時，極易面臨「小樣本資料稀缺」以及生成模型產生的「風格偏移（Style Drift）」問題。本研究提出一套名為 **GenNewSong** 的風格感知資料擴增框架，並基於擴增數據對 **GPT-2** 自回歸語言模型進行因果語言模型（Causal Language Modeling）微調。

研究跳脫傳統單純計算字元重疊的 BLEU 等指標，導入 **KL 散度（Kullback-Leibler Divergence）** 精確檢視生成資料與原始訓練集在調性、時序轉移上的風格機率分佈一致性。實驗結果證實，資料擴增對風格一致性具備**非單調（Non-monotonic）**之非線性影響，並成功找出 **約 3,000 至 12,000 筆** 的中等規模擴增訓練集，可在全域分佈一致性與局部文法轉移覆蓋率之間取得最佳平衡。

---

## Contributions

* **擴增框架參與開發：** 參與建構「GenNewSong」符號音樂擴增管線，將領域知識轉化為緩解 AI 小樣本資料稀缺之解決方案。
* **生成模型微調與分佈檢驗：** 執行 GPT-2 語言模型微調，並運用 KL 散度評估生成序列之分佈收斂性，發掘擴增資料規模對風格保持之非單調性規律。
* **專案統籌與通訊作者職責：** 擔任本論文之**通訊作者**，主導大會審查意見回覆、論文格式修改、行政聯繫與專案進度協調。

---

## Citation

若本研究對您的研究有所啟發，歡迎引用本篇論文：

```bibtex
@inproceedings{tseng2026style,
  title={Style-Aware Data Augmentation for Deep Learning on Symbolic Music},
  author={Tseng, Yung-Chi and Wang, Yu-Chia and Chen, Yung-An and Yang, Chin-Yun and Lin, Yu-Cheng},
  booktitle={Proceedings of the 2026 8th International Conference on Image, Video and Signal Processing (IVSP 2026)},
  year={2026},
  publisher={SPIE},
  doi={10.1117/12.3116024}
}
