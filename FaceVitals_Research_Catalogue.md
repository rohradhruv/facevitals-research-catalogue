# FaceVitals research catalogue

208 source-linked resources for research on RGB facial-video vital-sign estimation. Initial search: 13 October 2026; historical SP Cup update: 15 October 2026.

This is a broad scoping catalogue, not an exhaustive systematic review. Sources were located and triaged; not all full texts were read and methods were not reproduced. Vendor claims, preprints, special-hardware methods and unverified video links are identified.

[Official competition information](https://signalprocessingsociety.org/community-involvement/signal-processing-cup) · [Historical SP Cup review](Historical_SP_Cup/Past_SP_Cups_Relevance_to_FaceVitals.html)


## Foundations and classical signal processing


### R001 — Remote plethysmographic imaging using ambient light (GREEN; Verkruysse et al.)

2008 · Direct RGB · Paper

Essential green-channel baseline; ambient-light optical origin.

[Primary / author source](https://pmc.ncbi.nlm.nih.gov/articles/PMC2717852/)


### R002 — Non-contact, automated cardiac pulse measurements using video imaging and blind source separation (Poh et al.; ICA)

2010 · Direct RGB · Paper

Blind-source-separation baseline and early webcam pulse extraction.

[Primary / author source](https://dspace.mit.edu/entities/publication/f771f726-4f56-4f3f-9d57-70cb023fd02e)


### R003 — Robust pulse rate from chrominance-based rPPG (CHROM; de Haan and Jeanne)

2013 · Direct RGB · Paper

Core chrominance baseline; compare under motion and lighting changes.

[Primary / author source](https://pubmed.ncbi.nlm.nih.gov/23744659/)


### R004 — Improved motion robustness of remote-PPG by using the blood volume pulse signature (PBV)

2014 · Direct RGB · Paper

Physiological color-direction model; useful classical comparator.

[Primary / author source](https://pubmed.ncbi.nlm.nih.gov/25159049/)


### R005 — Algorithmic Principles of Remote PPG (POS; Wang et al.)

2016 online / 2017 print · Direct RGB · Paper

High-priority plane-orthogonal-to-skin baseline; also explains assumptions.

[Primary / author source](https://research.tue.nl/en/publications/algorithmic-principles-of-remote-ppg/)


### R006 — A Novel Algorithm for Remote Photoplethysmography: Spatial Subspace Rotation (2SR)

2015 online / 2016 print · Direct RGB · Paper

Spatial skin-color subspace alternative to channel averaging.

[Primary / author source](https://research.tue.nl/nl/publications/a-novel-algorithm-for-remote-photoplethysmography-spatial-subspac/)


### R007 — Local Group Invariance for Heart Rate Estimation From Face Videos in the Wild (LGI)

2018 · Direct RGB · Paper

Transformation-invariant extraction; relevant to uncontrolled conditions.

[Primary / author source](https://openaccess.thecvf.com/content_cvpr_2018_workshops/w27/html/Pilz_Local_Group_Invariance_CVPR_2018_paper.html)


### R008 — Real-Time Temporal Superpixels for Unsupervised Remote Photoplethysmography

2018 · Direct RGB · Paper

Region tracking and temporal aggregation for a practical pipeline.

[Primary / author source](https://openaccess.thecvf.com/content_cvpr_2018_workshops/w27/html/Bobbia_Real-Time_Temporal_Superpixels_CVPR_2018_paper.html)


### R009 — Face2PPG: An unsupervised pipeline for blood volume pulse extraction from faces (OMIT)

2022 preprint / 2023 publication · Direct RGB · Paper

Face stabilization, region selection and QR-based color transformation.

[Primary / author source](https://arxiv.org/abs/2202.04101)


### R010 — Eulerian Video Magnification for Revealing Subtle Changes in the World

2012 · Adjacent · Paper + code

Useful visualization and temporal filtering reference; magnified pulse is not a validated vital-sign estimate.

[Primary / author source](https://people.csail.mit.edu/mrub/evm/)


## Neural HR and waveform estimation


### R011 — DeepPhys: Video-Based Physiological Measurement Using Convolutional Attention Networks

2018 · Direct RGB · Paper

Foundational appearance/motion attention model; useful neural baseline.

[Primary / author source](https://openaccess.thecvf.com/content_ECCV_2018/html/Weixuan_Chen_DeepPhys_Video-Based_Physiological_ECCV_2018_paper.html)


### R012 — PhysNet: Remote Photoplethysmograph Signal Measurement Using Spatio-Temporal Networks

2019 · Direct RGB · Paper + code

3D spatiotemporal waveform baseline; do not confuse with molecular PhysNet.

[Primary / author source](https://github.com/ZitongYu/PhysNet)


### R013 — RhythmNet: End-to-end Heart Rate Estimation from Face via Spatial-temporal Representation

2019 preprint / 2020 journal · Direct RGB · Paper

Important spatial-temporal-map route to HR estimation.

[Primary / author source](https://arxiv.org/abs/1910.11515)


### R014 — Multi-Task Temporal Shift Attention Networks for On-Device Contactless Vitals Measurement (TS-CAN / MTTS-CAN)

2020 · Direct RGB · Paper

Efficient HR/respiration architecture; deployment-relevant comparator.

[Primary / author source](https://arxiv.org/abs/2006.03790)


### R015 — HeartTrack: Convolutional Neural Network for Remote Video-Based Heart Rate Monitoring

2020 · Direct RGB · Paper

Earlier video CNN approach; compare input processing and evaluation.

[Primary / author source](https://openaccess.thecvf.com/content_CVPRW_2020/papers/w19/Perepelkina_HeartTrack_Convolutional_Neural_Network_for_Remote_Video-Based_Heart_Rate_Monitoring_CVPRW_2020_paper.pdf)


### R016 — PulseGAN: Learning to Generate Realistic Pulse Waveforms in Remote Photoplethysmography

2020 preprint / 2021 publication · Direct RGB · Paper

Waveform reconstruction rather than just average HR.

[Primary / author source](https://arxiv.org/abs/2006.02699)


### R017 — Dual-GAN: Joint BVP and Noise Modeling for Remote Physiological Measurement

2021 · Direct RGB · Paper

Separates pulse and noise representations; robustness reference.

[Primary / author source](https://openaccess.thecvf.com/content/CVPR2021/papers/Lu_Dual-GAN_Joint_BVP_and_Noise_Modeling_for_Remote_Physiological_Measurement_CVPR_2021_paper.pdf)


### R018 — The Way to My Heart Is Through Contrastive Learning: Remote Photoplethysmography From Unlabelled Video

2021 · Direct RGB · Paper

Self-supervised learning when aligned waveform labels are limited.

[Primary / author source](https://openaccess.thecvf.com/content/ICCV2021/html/Gideon_The_Way_to_My_Heart_Is_Through_Contrastive_Learning_Remote_ICCV_2021_paper.html)


### R019 — Non-contact PPG Signal and Heart Rate Estimation with Multi-hierarchical Convolutional Network

2021 · Direct RGB · Paper

Motion-aware ROI and multiscale feature extraction.

[Primary / author source](https://arxiv.org/abs/2104.02260)


### R020 — PhysFormer: Facial Video-based Physiological Measurement with Temporal Difference Transformer

2022 · Direct RGB · Paper + code

Strong transformer comparison; more complex than classical baselines.

[Primary / author source](https://arxiv.org/abs/2111.12082) · [Code / related source](https://github.com/ZitongYu/PhysFormer)


### R021 — Contrast-Phys: Unsupervised Video-based Remote Physiological Measurement via Spatiotemporal Contrast

2022 · Direct RGB · Paper + code

Unsupervised pulse learning; requires careful spectral validation.

[Primary / author source](https://arxiv.org/abs/2208.04378) · [Code / related source](https://github.com/zhaodongsun/contrast-phys)


### R022 — EfficientPhys: Enabling Simple, Fast and Accurate Camera-Based Cardiac Measurement

2023 · Direct RGB · Paper

High-priority lightweight neural candidate for live inference.

[Primary / author source](https://openaccess.thecvf.com/content/WACV2023/html/Liu_EfficientPhys_Enabling_Simple_Fast_and_Accurate_Camera-Based_Cardiac_Measurement_WACV_2023_paper.html)


### R023 — Non-Contrastive Unsupervised Learning of Physiological Signals From Video (SiNC)

2023 · Direct RGB · Paper

Frequency-based unsupervised learning; compare with supervised models.

[Primary / author source](https://openaccess.thecvf.com/content/CVPR2023/html/Speth_Non-Contrastive_Unsupervised_Learning_of_Physiological_Signals_From_Video_CVPR_2023_paper.html)


### R024 — Contrast-Phys+: Unsupervised and Weakly-supervised Video-based Remote Physiological Measurement

2023 preprint / 2024 journal · Direct RGB · Paper + code

Handles partial or misaligned supervision; RGB and NIR experiments must be separated.

[Primary / author source](https://arxiv.org/abs/2309.06924) · [Code / related source](https://github.com/zhaodongsun/contrast-phys)


### R025 — rPPG-MAE: Self-supervised Pretraining with Masked Autoencoders for Remote Physiological Measurements

2024 · Direct RGB · Paper + code

Representation pretraining; code includes STMap preparation guidance.

[Primary / author source](https://github.com/keke-nice/rPPG-MAE)


### R026 — FactorizePhys: Matrix Factorization for Multidimensional Attention in Remote Physiological Sensing

2024 · Direct RGB · Paper + code

Matrix-factorization attention; useful modern neural comparator.

[Primary / author source](https://arxiv.org/abs/2411.01542) · [Code / related source](https://github.com/PhysiologicAILab/FactorizePhys)


### R027 — PhysMamba (dual-stream spatiotemporal Mamba for remote physiological measurement)

2024 · Direct RGB · Paper + code

State-space architecture; verify dependencies and inference footprint.

[Primary / author source](https://github.com/Chaoqi31/PhysMamba)


### R028 — RhythmMamba: Fast Remote Physiological Measurement with Arbitrary Length Videos

2024 preprint / 2025 conference · Direct RGB · Paper + code

State-space model with arbitrary-length video handling.

[Primary / author source](https://arxiv.org/abs/2404.06483) · [Code / related source](https://github.com/zizheng-guo/RhythmMamba)


### R029 — RhythmFormer: Extracting Patterned rPPG Signals Based on Periodic Sparse Attention

2024 preprint / 2025 journal · Direct RGB · Paper + code

Periodicity-aware attention; study accuracy/runtime tradeoff.

[Primary / author source](https://github.com/zizheng-guo/RhythmFormer)


### R030 — BeatFormer: Efficient motion-robust remote heart rate estimation through unsupervised spectral learning

2025 · Direct RGB · Paper

Recent efficient and motion-focused method.

[Primary / author source](https://openaccess.thecvf.com/content/ICCV2025W/CVPM/html/Martinez_BeatFormer_Efficient_motion-robust_remote_heart_rate_estimation_through_unsupervised_spectral_ICCVW_2025_paper.html)


### R031 — RhythmGuassian: Repurposing Generalizable Gaussian Model For Remote Physiological Measurement

2025 · Direct RGB · Paper

Gaussian-model approach; title spelling follows the CVF record.

[Primary / author source](https://openaccess.thecvf.com/content/ICCV2025/html/Lu_RhythmGuassian_Repurposing_Generalizable_Gaussian_Model_For_Remote_Physiological_Measurement_ICCV_2025_paper.html)


### R032 — PHASE-Net: Physics-Grounded Harmonic Attention System for Efficient Remote Photoplethysmography Measurement

2026 · Direct RGB · Paper

Recent physics-informed harmonic attention; verify full experimental protocol before choosing.

[Primary / author source](https://openaccess.thecvf.com/content/CVPR2026/papers/Zhao_PHASE-Net_Physics-Grounded_Harmonic_Attention_System_for_Efficient_Remote_Photoplethysmography_Measurement_CVPR_2026_paper.pdf)


### R033 — rPPG-VQA: A Video Quality Assessment Framework for Unsupervised rPPG Training

2026 · Direct RGB · Paper

Training-time video-quality assessment; relevant to quality-aware learning.

[Primary / author source](https://openaccess.thecvf.com/content/CVPR2026/html/Dai_rPPG-VQA_A_Video_Quality_Assessment_Framework_for_Unsupervised_rPPG_Training_CVPR_2026_paper.html)


### R034 — PhysNeXt: Next-Generation Dual-Branch Structured Attention Fusion Network for Remote Photoplethysmography Measurement

2026 preprint · Direct RGB · Preprint

New architecture lead; not a reproduced baseline in this catalogue.

[Primary / author source](https://arxiv.org/abs/2603.19752)


### R035 — FCUS-rPPG: A Fast-Converging Unsupervised Framework for Remote Photoplethysmography via Gradient Oscillation Suppression

2026 preprint · Direct RGB · Preprint

Recent rPPG learning lead; full methodology review remains necessary.

[Primary / author source](https://arxiv.org/abs/2606.03050)


### R036 — Rhythm-Structured Predictive Learning for Remote Photoplethysmography (RhythmJEPA)

2026 preprint · Direct RGB · Preprint

Recent representation-learning lead; publication status not assumed.

[Primary / author source](https://arxiv.org/abs/2606.31736)


### R037 — TDA-Phys: Temporal Difference Adaptation of Video Foundation Model for Remote Photoplethysmography

2026 · Direct RGB · Paper

Adapts video foundation models; assess compute cost before adopting.

[Primary / author source](https://www.mdpi.com/2076-3417/16/4/2038)


## SpO2 and multi-vital estimation


### R038 — Camera-based pulse-oximetry using adaptive PBV (van Gastel et al.)

2016 · Adjacent: special optics · Paper

Near-infrared wavelength setup; physiological reference, not a plain RGB webcam solution.

[Primary / author source](https://www.nature.com/articles/srep38609)


### R039 — Contactless SpO2 with calibrated RGB camera / optical system

2022 · Conditional RGB hardware · Paper

RGB oxygenation study with calibration and added optical/illumination hardware; check setup compatibility.

[Primary / author source](https://pmc.ncbi.nlm.nih.gov/articles/PMC9774849/)


### R040 — Evaluating the robustness of a contactless SpO2 estimation approach to head movements

2022 online / 2023 issue · Direct RGB · Paper

SpO2 motion-robustness study; inspect calibration and label range.

[Primary / author source](https://pmc.ncbi.nlm.nih.gov/articles/PMC8758222/)


### R041 — Contactless Blood Oxygen Saturation Estimation from Facial Videos Using Deep Learning

2024 · Direct RGB · Paper

High-priority facial SpO2 study using VIPL-HR and STMaps.

[Primary / author source](https://pmc.ncbi.nlm.nih.gov/articles/PMC10968547/)


### R042 — Blood Oxygen Saturation Estimation from Facial Video via DC and AC components of Spatio-temporal Map

2022 preprint · Direct RGB · Preprint

Oxygenation-oriented DC and AC information; title/details should be taken from linked record.

[Primary / author source](https://arxiv.org/abs/2212.07116)


### R043 — Remote Blood Oxygen Estimation From Videos Using Neural Networks

2021 preprint · Review input region · Preprint

Related oxygenation learning; verify capture region and hardware before treating as facial baseline.

[Primary / author source](https://arxiv.org/abs/2107.05087)


### R044 — Multi-Channel Ratio-of-Ratios for Noncontact Hand Video Based SpO2 Monitoring

2021 preprint · Adjacent: hand video · Preprint

Ratio-of-ratios idea; hand input does not directly meet facial-video scope.

[Primary / author source](https://arxiv.org/abs/2107.08528)


### R045 — Camera Measurement of Blood Oxygen Saturation

2025 preprint · Review hardware · Preprint

Recent oxygenation lead; do not assume off-the-shelf facial RGB compatibility.

[Primary / author source](https://arxiv.org/abs/2503.01699)


### R046 — Video-based SpO2 estimation in multiple scenarios with wavelength-guided modeling

2026 · Review hardware · Paper

Recent SpO2 approach; read wavelength and calibration assumptions carefully.

[Primary / author source](https://www.sciencedirect.com/science/article/pii/S1746809426004714)


### R047 — Random Forest-Based Blood Oxygen Saturation Estimation System Using a Web Camera

2026 · Direct RGB lead · Paper

Recent journal lead; inspect population and reference distribution before reuse.

[Primary / author source](https://www.jstage.jst.go.jp/article/abe/15/0/15_254/_article/-char/en)


### R048 — Addressing Healthcare Needs of the Elderly in Contactless Blood Oxygen Saturation Estimation

2024 · Direct RGB · Paper

Age-specific SpO2 evidence; relevant to C6, not merely HR accuracy.

[Primary / author source](https://www.eee.hku.hk/optima/pub/conference/2401_PWc.pdf)


### R049 — Remote Photoplethysmography for Contactless Blood Oxygen Saturation Monitoring

2024 · Direct RGB lead · Paper

Elderly/assisted-living motivation; inspect full validation and setup.

[Primary / author source](https://ieeexplore.ieee.org/iel8/10676995/10677018/10677187.pdf)


### R050 — ReViSe: Remote Vital Signs Measurement Using Smartphone Camera

2022 preprint · Direct RGB · Preprint

Especially relevant integrated HR/HRV/SpO2/BP system; check independent-subject validation.

[Primary / author source](https://arxiv.org/abs/2206.08748)


## Blood pressure estimation


### R051 — Smartphone-Based Blood Pressure Measurement Using Transdermal Optical Imaging Technology (Luo et al.)

2019 · Direct RGB · Paper

Foundational facial BP study; normotensive cohort limits generalization to hypertensive patients.

[Primary / author source](https://pubmed.ncbi.nlm.nih.gov/31382766/)


### R052 — Robust blood pressure estimation using an RGB camera (Fan et al.)

2018 online / 2020 issue · Direct RGB · Paper

Early facial RGB BP approach; assess calibration and subject split.

[Primary / author source](https://link.springer.com/article/10.1007/s12652-018-1026-6)


### R053 — Assessment of deep learning based blood pressure prediction from PPG and rPPG signals

2021 preprint · Direct + contact comparison · Preprint

Important cautionary comparison of signal sources and evaluation choices.

[Primary / author source](https://arxiv.org/abs/2104.09313)


### R054 — Remote blood pressure measurement via spatiotemporal mapping of a short-time facial video

2022 preprint · Direct RGB · Preprint

Facial BP approach; inspect private-data availability and subject leakage.

[Primary / author source](https://arxiv.org/abs/2203.03634)


### R055 — Ensemble deep learning for blood pressure estimation using facial videos

2024 · Direct RGB · Paper

Ensemble BP predictor; author-hosted manuscript and RePSS context.

[Primary / author source](https://liangli-zhen.github.io/assets/pdf/RePPS_BP.pdf)


### R056 — Remote Blood Pressure Estimation from Facial Videos using Transfer Learning: Leveraging PPG to rPPG Conversion

2025 · Direct RGB + contact training · Paper

High-priority transfer-learning approach; contact teacher does not mean contact inference.

[Primary / author source](https://openaccess.thecvf.com/content/WACV2025/papers/Cheng_Remote_Blood_Pressure_Estimation_from_Facial_Videos_using_Transfer_Learning_WACV_2025_paper.pdf)


### R057 — Estimating Blood Pressure with a Camera: An Exploratory Study of Ambulatory Patients with Cardiovascular Disease

2025 preprint · Direct RGB · Preprint

Disease-cohort evidence; valuable counterpoint to healthy-only studies.

[Primary / author source](https://arxiv.org/abs/2503.00890)


### R058 — Phase-shifted remote photoplethysmography for estimating heart rate and blood pressure from facial video (DRP-Net / BBP-Net)

2026 journal / 2024 preprint · Conditional: training inputs · Paper

Facial/acral supervision is discussed; establish exactly which inputs are needed at deployment.

[Primary / author source](https://www.sciencedirect.com/science/article/abs/pii/S0263224126009498) · [Code / related source](https://arxiv.org/abs/2401.04560)


### R059 — BP-rPPG: An Indian Face-Video Dataset and PPG-Guided Baseline for Remote Blood Pressure Estimation (ALIVE)

2026 · Direct RGB + contact teacher · Paper + code + data request

Very relevant Indian BP resource; inspect subject split, label range and data-use agreement.

[Primary / author source](https://dspace.iiti.ac.in/handle/123456789/19013) · [Code / related source](https://github.com/TrishnaSaikia/BP-rPPG-ALIVE)


### R060 — A Pulse-Feature LSTM Framework with Temporal Variance-Based Prediction Filtering for rPPG-Based Blood Pressure Estimation

2026 · Direct RGB · Paper

Morphological features plus temporal filtering; check withheld failure rates.

[Primary / author source](https://www.mdpi.com/2079-9292/15/17/3862)


### R061 — Feasibility and Evaluation of Effective Morphological Feature Representation for Contactless Blood Pressure Estimation Using Remote Photoplethysmography

2026 · Direct RGB · Paper

Useful study of whether recoverable morphology supports BP prediction.

[Primary / author source](https://www.mdpi.com/2079-9292/15/17/3864)


### R062 — A hybrid machine learning and deep learning framework for non-invasive blood pressure estimation from rPPG signals

2026 · Review sensor requirements · Paper

PTT/Transformer/LSTM approach; determine whether extra timing/sensor inputs are required.

[Primary / author source](https://www.sciencedirect.com/science/article/pii/S1746809426012449)


### R063 — CALM-BP: Observation-Matched Physiological Semantic Grounding for Non-Contact Blood Pressure Estimation

2026 preprint · Direct rPPG lead · Preprint

New semantic-grounding approach; private FlowBP-Set availability needs checking.

[Primary / author source](https://arxiv.org/abs/2608.21744)


## Datasets and data access


### R064 — UBFC-rPPG (Dataset 1 and Dataset 2)

2017/2018 · Direct RGB · Dataset

Start here for HR. Dataset 1 has SpO2 in its documented dump; do not assume Dataset 2 contains SpO2.

[Primary / author source](https://sites.google.com/view/ybenezeth/ubfcrppg)


### R065 — PURE: Pulse Rate Detection Dataset

2014 · Direct RGB · Dataset

Controlled motion benchmark; label channels and licensing must be inspected in release.

[Primary / author source](https://www.tu-ilmenau.de/en/university/departments/department-of-computer-science-and-automation/profile/institutes-and-groups/institute-of-computer-and-systems-engineering/group-for-neuroinformatics-and-cognitive-robotics/data-sets-code)


### R066 — COHFACE

2016 · Direct RGB · Dataset

RGB, synchronized BVP and breathing; useful compressed-video HR benchmark, not a three-vital dataset.

[Primary / author source](https://www.idiap.ch/en/dataset/cohface)


### R067 — VIPL-HR

2018 · Direct RGB subset · Dataset request

RGB plus NIR recordings; SpO2 recorded. Use RGB subset and verify saturation range and timing.

[Primary / author source](https://vipl.ict.ac.cn/resources/databases/201811/t20181129_32716.html)


### R068 — VIPL-HR-V2

2020 · Direct RGB lead · Dataset request

Expanded HR resource; access through lab/author agreement. Verify actual downloadable modalities and labels.

[Primary / author source](https://sites.google.com/site/huhanhomepage/datasetcode)


### R069 — UBFC-Phys

2021 · Direct RGB · Dataset

Stress-task video and physiological references; different resource from UBFC-rPPG.

[Primary / author source](https://sites.google.com/view/ybenezeth/ubfc-phys)


### R070 — MMPD: Multi-Domain Mobile Video Physiology Dataset

2023 · Direct RGB · Paper + dataset request

Skin-tone, lighting and motion diversity; high-priority generalization benchmark.

[Primary / author source](https://arxiv.org/abs/2302.03840) · [Code / related source](https://github.com/McJackTang/MMPD_rPPG_dataset)


### R071 — SCAMPS: Synthetics for Camera Measurement of Physiological Signals

2022 · Synthetic RGB · Paper + dataset

Synthetic pulse/respiration and segmentation; useful training supplement, not clinical test evidence.

[Primary / author source](https://arxiv.org/abs/2206.04197) · [Code / related source](https://github.com/danmcduff/scampsdataset)


### R072 — iBVP: RGB-Thermal rPPG Dataset with High Resolution Signal Quality Labels

2024 · Direct RGB subset · Paper + dataset

Use RGB alone at inference; dense signal-quality annotations are useful.

[Primary / author source](https://github.com/PhysiologicAILab/iBVP-Dataset)


### R073 — BP4D+ Multimodal Spontaneous Emotion Corpus

2016 · Direct video subset · Dataset request

Facial video and rich physiology including BP; check BP channel meaning, units and synchronization.

[Primary / author source](https://www.cs.binghamton.edu/~lijun/Research/3DFE/3DFE_Analysis.html)


### R074 — V4V: Vision for Vitals dataset and challenge

2021 · Direct RGB · Paper + dataset lead

Naturalistic facial behavior, HR/respiration and physiological channels; confirm released BP access.

[Primary / author source](https://openaccess.thecvf.com/content/ICCV2021W/V4V/papers/Revanur_The_First_Vision_for_Vitals_V4V_Challenge_for_Non-Contact_Video-Based_ICCVW_2021_paper.pdf)


### R075 — OBF: Oulu Bio-Face database

2018 · Direct RGB subset · Paper + dataset request

Healthy and atrial-fibrillation cohorts with physiological references; valuable clinical-domain HR evidence.

[Primary / author source](https://oulurepo.oulu.fi/handle/10024/25678)


### R076 — LGI-PPGI database

2018 · Direct RGB · Dataset lead

Realistic-condition recordings associated with LGI; check the release and per-session ground truth.

[Primary / author source](https://github.com/partofthestars/LGI-PPGI-DB)


### R077 — AiPEX-Lab rPPG representation-bias data

2021 · Direct RGB · Paper + dataset

India and Sierra Leone data; competition-annexure resource for demographic robustness.

[Primary / author source](https://www.nature.com/articles/s41746-021-00462-z) · [Code / related source](https://github.com/AiPEX-Lab/rppg_biases)


### R078 — SUMS: Summit Vitals multi-camera and multi-signal high-altitude dataset

2024 · Facial RGB subset only · Paper + data request

Face and finger videos with SpO2; face+finger fusion results do not satisfy facial-only inference. Faculty agreement required.

[Primary / author source](https://arxiv.org/abs/2409.19223) · [Code / related source](https://github.com/thuhci/SUMS)


### R079 — LADH: Long-term Altitude Daily Health / FusionVitals

2025 · RGB subset only · Paper + data request

Daily-care occlusion/pose, RGB/IR and SpO2. RGB+IR improvements are not transferable without testing RGB-only.

[Primary / author source](https://arxiv.org/abs/2506.09718) · [Code / related source](https://github.com/McJackTang/FusionVitals)


### R080 — PhysDrive: Multimodal Remote Physiological Measurement Dataset for In-vehicle Driver Monitoring

2025 · RGB subset only · Paper + data request

Driving/lighting variation; ECG/BVP/SpO2 references. NIR/radar inference is outside our RGB solution.

[Primary / author source](https://github.com/WJULYW/PhysDrive-Dataset)


### R081 — MCD-rPPG / Gaze into the Heart: A Multi-View Video Dataset for rPPG and Health Biomarkers Estimation

2025 paper · Facial RGB · Paper + data lead

Multi-view video and biomarkers including BP/SpO2; verify alignment, units and data-access host.

[Primary / author source](https://arxiv.org/abs/2508.17924) · [Code / related source](https://github.com/ksyegorov/mcd_rppg)


### R082 — VitalVideos-Europe-1

Original release; see provider · Facial RGB · Dataset request

Provider lists HR/PPG/SpO2/BP; academic subset access requires signed request.

[Primary / author source](https://www.vitalvideos.org/)


### R083 — VitalVideos-Africa-1

See provider · Facial subset only · Dataset request

Useful skin-tone coverage; some recordings include palms, so select eligible facial input.

[Primary / author source](https://www.vitalvideos.org/)


### R084 — VitalVideos-Worldwide

2025 · Facial RGB · Paper + dataset request

Rich HR/SpO2/BP ground truth across regions. Paper says 7000 participants; current site says 6500+, so release/version counts need confirmation.

[Primary / author source](https://openaccess.thecvf.com/content/ICCV2025W/CVPM/html/Toye_VitalVideos-Worldwide_A_large_and_diverse_rPPG_dataset_with_rich_ground_ICCVW_2025_paper.html) · [Code / related source](https://huggingface.co/datasets/pjtoye/VitalVideos-Worldwide)


### R085 — VitalVideos-SpO2 and Longitudinal collections

See provider · Facial RGB · Dataset request

Small specialized oxygenation and repeated-session data leads; verify accessible subset and terms.

[Primary / author source](https://www.vitalvideos.org/)


### R086 — CHILL low-illumination / elevated-heart-rate dataset

2025 study · Direct RGB · Dataset lead

Real low-light recordings; useful C1 evidence beyond synthetic darkening.

[Primary / author source](https://www.uni-bielefeld.de/fakultaeten/technische-fakultaet/arbeitsgruppen/human-centered-artificial-intelligence/research/rppg/)


### R087 — Masked/unmasked pulse-estimation datasets (Speth et al.)

2021 · Direct RGB · Paper + dataset lead

Study reports real masked recordings and synthetic-mask augmentation; access must be checked. Also a high-priority C7 methods paper.

[Primary / author source](https://arxiv.org/abs/2101.04096)


### R088 — HiDURPA and resolution-aware compression study materials

See project page · Direct RGB · Dataset lead

High-definition uncompressed capture and codec experiments; useful C4/C5 reference.

[Primary / author source](https://www.eah-jena.de/vitawave/publications/videocompressionrppg)


### R089 — Organizer clinical dataset: Sri Ramachandra Hospital

2027 competition document · Direct RGB intended · Restricted organizer data

Explicitly described in official PDF FAQ; dataset agreement and primary-organizer contact required. Not downloaded here.

[Primary / author source](https://signalprocessingsociety.org/community-involvement/signal-processing-cup)


## Toolboxes, code and implementation references


### R090 — rPPG-Toolbox

2023 paper / maintained repo · Direct RGB · Paper + Python code

Primary recommended benchmark framework; use original ubicomplab repository and pinned configs.

[Primary / author source](https://arxiv.org/abs/2210.00716) · [Code / related source](https://github.com/ubicomplab/rPPG-Toolbox)


### R091 — pyVHR: a Python framework for remote photoplethysmography

2022 paper · Direct RGB · Paper + Python code

Useful ROI and classical-method experimentation; paper states GPL-3.0, inspect license before redistribution.

[Primary / author source](https://pmc.ncbi.nlm.nih.gov/articles/PMC9044207/) · [Code / related source](https://github.com/phuselab/pyVHR)


### R092 — iPhys: An Open Non-Contact Imaging-Based Physiological Measurement Toolbox

2019 · Direct RGB · Paper + MATLAB code

Classical MATLAB baseline reference; appropriate to our Python/MATLAB skill set.

[Primary / author source](https://arxiv.org/abs/1901.04366) · [Code / related source](https://github.com/danmcduff/iphys-toolbox)


### R093 — Remote Bio-Sensing: Open Source Benchmark Framework for Fair Evaluation of rPPG

2023 preprint · Direct + adjacent modules · Paper + Python code

Useful alternative benchmark; separate facial rPPG modules from contact-PPG/BP modules.

[Primary / author source](https://arxiv.org/abs/2307.12644) · [Code / related source](https://github.com/remotebiosensing/rppg)


### R094 — Open-rppg (KegangWangCCNU)

Maintained repo · Direct RGB · Python code

Implementation/API resource; independently validate outputs before reuse.

[Primary / author source](https://github.com/KegangWangCCNU/open-rppg)


### R095 — Open-rppg (chnbld)

Maintained repo · Direct RGB · Python code

Different project sharing a similar name; exposes HR and signal-quality outputs.

[Primary / author source](https://github.com/chnbld/open-rppg)


### R096 — Motion Matters: Neural Motion Transfer for Better Camera Physiological Sensing / MA-rPPG Video Toolbox

2024 · Synthetic augmentation · Python code

Motion augmentation linked by rPPG-Toolbox; preserve subject split before generating variants.

[Primary / author source](https://github.com/yahskapar/MA-rPPG-Video-Toolbox)


### R097 — MMRPhys: Multi-Modal Multi-Task Remote Physiological Sensing

See repo · RGB-compatible modules · Python code

Useful common model/data implementation; multimodal settings need RGB-only configuration.

[Primary / author source](https://github.com/PhysiologicAILab/MMRPhys)


### R098 — rPPG-SDK (pranav8431)

Community repo · Unvalidated demo · Python code

Community integrated-vitals demo; SpO2 claims are not clinical-validation evidence.

[Primary / author source](https://github.com/pranav8431/rPPG-SDK)


### R099 — MediaPipe Face Landmarker

Current documentation · Enabling technology · Official docs

Face landmarks and ROI construction; not a vitals estimator.

[Primary / author source](https://ai.google.dev/edge/mediapipe/solutions/vision/face_landmarker)


### R100 — MATLAB face detection and tracking / CamShift example

Current documentation · Enabling technology · Official docs

Official implementation reference explicitly listed by competition.

[Primary / author source](https://www.mathworks.com/help/vision/ug/face-detection-and-tracking-using-camshift.html)


### R101 — MATLAB designfilt

Current documentation · Enabling technology · Official docs

Official bandpass-filter design reference from competition resources.

[Primary / author source](https://www.mathworks.com/help/signal/ref/designfilt.html)


### R102 — FFmpeg documentation

Current documentation · Enabling technology · Official docs

Reproducible bitrate/fps/codec stress tests; measure actual output bitrate rather than assuming quality slider equals kbps.

[Primary / author source](https://ffmpeg.org/documentation.html)


## Robustness, fairness and deployment studies


### R103 — A Novel Framework for Remote Photoplethysmography Pulse Extraction on Compressed Videos

2018 · Direct RGB · Paper

Classical compression-aware signal extraction.

[Primary / author source](https://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w27/Zhao_A_Novel_Framework_CVPR_2018_paper.pdf)


### R104 — Remote Photoplethysmography with Spatial-Temporal Enhancement for Compressed Videos (STVEN / rPPGNet)

2019 · Direct RGB · Paper + code

Video enhancement and compressed-video physiology extraction.

[Primary / author source](https://github.com/ZitongYu/STVEN_rPPGNet)


### R105 — Remote physiological measurement with arbitrary video resolution

2022 preprint · Direct RGB · Paper + code

Relevant to C4; distinguish original-frame resolution from neural input resize.

[Primary / author source](https://arxiv.org/abs/2211.16922) · [Code / related source](https://github.com/LJW-GIT/Arbitrary_Resolution_rPPG)


### R106 — Federated Remote Physiological Measurement with Imperfect Data

2022 · Direct RGB · Paper

Decentralized training and imperfect data; not a substitute for offline inference testing.

[Primary / author source](https://openaccess.thecvf.com/content/CVPR2022W/CVPM/html/Liu_Federated_Remote_Physiological_Measurement_With_Imperfect_Data_CVPRW_2022_paper.html)


### R107 — Examining the Effects of Compression on Deep Learning Remote Photoplethysmography

2024 · Direct RGB · Paper

TS-CAN codec sensitivity; useful low-bandwidth experimental design.

[Primary / author source](https://library.imaging.org/admin/apis/public/api/ist/website/downloadArticle/ei/36/10/IPAS-248)


### R108 — A comprehensive evaluation of multiple video compression algorithms for preserving BVP signal quality

2024 online · Direct RGB · Paper

Codec, bitrate-control and GOP effects; avoid treating all H.264 settings as equivalent.

[Primary / author source](https://www.sciencedirect.com/science/article/pii/S1746809424015039)


### R109 — The reliability of remote photoplethysmography under low illumination and elevated heart rates

2025 · Direct RGB · Paper

Compares classical/neural methods and CHILL; useful realistic C1 stress evidence.

[Primary / author source](https://pmc.ncbi.nlm.nih.gov/articles/PMC12678791/)


### R110 — The role of face regions in remote photoplethysmography for contactless heart rate monitoring

2025 · Direct RGB · Review

ROI evidence; relevant to mask-safe forehead/cheek selection.

[Primary / author source](https://pmc.ncbi.nlm.nih.gov/articles/PMC12297079/)


### R111 — Demographic bias in public remote photoplethysmography datasets

2025 · Direct RGB · Review

Dataset representation and fairness gaps; pooled accuracy is insufficient.

[Primary / author source](https://pmc.ncbi.nlm.nih.gov/articles/PMC12491395/)


### R112 — Inclusive Contactless Monitoring for Older Adults From Diverse Backgrounds: Mixed Methods Study

2026 · Direct RGB context · Paper

Older-adult feasibility and acceptability evidence; access-limited human data.

[Primary / author source](https://pmc.ncbi.nlm.nih.gov/articles/PMC13330646/)


### R113 — Remote Photoplethysmography System for Vital Signs Estimation: Perceived Usability Evaluation by Elderly People

2025 · Deployment context · Paper

Usability evidence rather than proof of three-vital accuracy.

[Primary / author source](https://personales.upv.es/thinkmind/SPWID/SPWID_2025/spwid_2025_1_10_80007.html)


### R114 — Study on Real-Time Heart Rate Detection Based on Multi-People

2023 · Direct RGB · Paper

C3-related tracking/HR work; separately test persistent designated-target identity.

[Primary / author source](https://www.techscience.com/csse/v44n2/48288/html)


### R115 — Recovery-Aware Learning for Remote Photoplethysmography During Post-Exercise Heart Rate Recovery

2026 · Direct RGB · Paper

Temporal dynamics and MCD-rPPG evaluation; useful non-resting HR reference.

[Primary / author source](https://www.mdpi.com/2079-9292/15/18/4221)


## Reviews and field maps


### R116 — RGB Camera-based Physiological Sensing: Challenges and Future Directions

2021 preprint · Field map · Review

Broad camera-physiology roadmap; good initial reading.

[Primary / author source](https://arxiv.org/abs/2110.13362)


### R117 — Intelligent Remote Photoplethysmography-Based Methods for Heart Rate Estimation from Face Videos: A Survey

2022 · Field map · Review

Neural-method and dataset overview.

[Primary / author source](https://www.mdpi.com/2227-9709/9/3/57)


### R118 — Remote photoplethysmography for heart rate measurement: A review

2023/2024 · Field map · Review

HR methods and practical limitations; not evidence for a particular BP claim.

[Primary / author source](https://www.sciencedirect.com/science/article/pii/S1746809423010418)


### R119 — Review on remote heart rate measurements using photoplethysmography

2023 online / 2024 issue · Field map · Review

Classical and learning-method context.

[Primary / author source](https://link.springer.com/article/10.1007/s11042-023-16794-9)


### R120 — A comprehensive review of heart rate measurement using remote photoplethysmography and deep learning

2025 · Field map · Review

Useful neural-model and dataset bibliography.

[Primary / author source](https://pmc.ncbi.nlm.nih.gov/articles/PMC12181896/)


### R121 — Advancements in Remote Photoplethysmography

2025 · Field map · Review

Methods and dataset comparison; primary papers remain the evidence for model claims.

[Primary / author source](https://www.mdpi.com/2079-9292/14/5/1015)


### R122 — Remote photoplethysmography for camera-based vital sign estimation: A systematic literature review, challenges and deployment guidelines

2026 · Field map · Review

Recent multi-vital/deployment overview.

[Primary / author source](https://www.sciencedirect.com/science/article/pii/S2590005626002924)


### R123 — Roadmap of remote photoplethysmography from heart rate measurement toward clinical translation

2026 · Field map · Review

High-priority assessment of what separates lab HR results from clinical deployment.

[Primary / author source](https://www.nature.com/articles/s41746-026-02715-1)


### R124 — Smartphones and Video Cameras: Future Methods for Blood Pressure Measurement

2021 · BP field map · Review

BP physiology, camera approaches and validation concerns.

[Primary / author source](https://pmc.ncbi.nlm.nih.gov/articles/PMC8633391/)


### R125 — Representation biases in remote photoplethysmography datasets: a narrative review

2025/2026 · Fairness field map · Review

Additional demographic-coverage bibliography; check actual publication record.

[Primary / author source](https://doi.org/10.1108/ACI-06-2025-0270)


## Earlier challenges and proceedings


### R126 — The 2nd Challenge on Remote Physiological Signal Sensing (RePSS)

2021 · Direct RGB · Challenge report

Benchmark protocols and previous approaches; expand through cited submissions.

[Primary / author source](https://openaccess.thecvf.com/content/ICCV2021W/RePSS/papers/Li_The_2nd_Challenge_on_Remote_Physiological_Signal_Sensing_RePSS_ICCVW_2021_paper.pdf)


### R127 — RePSS 2024 proceedings: vision-based HR and blood pressure tracks

2024 · Direct RGB · Proceedings

Very relevant prior competition solutions, including CNN/random-forest BP work.

[Primary / author source](https://ceur-ws.org/Vol-3750/)


### R128 — The 3rd RePSS Track 2 data and rules

2024 · Direct RGB · Challenge data lead

Facial video/PPG/BP; its competition-only data permission must not be assumed valid for SP Cup.

[Primary / author source](https://www.kaggle.com/competitions/the-3rd-repss-t2/data)


## Existing products and comparable implementations


### R129 — NuraLogix Anura / transdermal optical imaging

Current product · Proprietary RGB system · Vendor source

Comparable facial multi-vital product. Vendor claims require parameter-specific independent evidence.

[Primary / author source](https://nuralogix.ai/anura-for-telemedicine/)


### R130 — Binah.ai SDK and research reports

Current product · Proprietary RGB system · Vendor source

Comparable HR/SpO2/BP software; resting/well-lit instructions differ from our stress conditions.

[Primary / author source](https://www.binah.ai/research/)


### R131 — FaceHeart Vitals SDK

Current product · Proprietary RGB system · Vendor source

Vendor identifies FDA clearance for HR and respiration; do not extend that clearance to BP/SpO2.

[Primary / author source](https://faceheart.com/products/faceheart-vitals-sdk)


### R132 — Shen AI

Current product · Proprietary camera system · Vendor source

Comparable camera-health platform; exact parameter support/validation needs product documentation review.

[Primary / author source](https://shen.ai/about-us)


### R133 — PanopticAI Vitals SDK

Current product · Proprietary camera system · Vendor docs

Comparable implementation and documentation; linked 2024 facial SpO2 paper is stronger scientific evidence.

[Primary / author source](https://docs.panoptic.ai/)


### R134 — Oxehealth contactless monitoring

Current product · Adjacent room monitoring · Vendor source

Deployment comparison; do not assume its camera/hardware setup matches facial RGB competition input.

[Primary / author source](https://www.oxehealth.com/how-it-helps)


### R135 — Heart Vision: Privacy-Preserving Digital Health Biomarkers for Elderly People (FAU project)

2023 · Direct RGB demo · University project

Comparable student project using pyVHR; does not establish clinical three-vital performance.

[Primary / author source](https://www.fau.edu/engineering/senior-design/projects/summer2023/privacy-preserving-digital-health/)


## Discovery indexes and additional leads


### R136 — Awesome-rPPG (seven0813)

Living index · Discovery only · Community bibliography

Expand cited papers and datasets; index inclusion is not validation.

[Primary / author source](https://github.com/seven0813/Awesome-rPPG)


### R137 — Awesome-rPPG (zx-pan)

Living index · Discovery only · Community bibliography

Second bibliography for citation snowballing; deduplicate papers and forks.

[Primary / author source](https://github.com/zx-pan/Awesome-rPPG)


### R138 — rPPG-Trends (Z-Xiong)

Living index · Discovery only · Community bibliography

Toolbox and product discovery; verify original sources.

[Primary / author source](https://github.com/Z-Xiong/rPPG-Trends)


### R139 — GitHub rppg topic

Living index · Discovery only · Repository discovery

Find projects and author repositories; stars do not establish accuracy.

[Primary / author source](https://github.com/topics/rppg)


### R140 — Non-contact measurement system for COVID-19 vital signs to aid mass screening: An alternate approach

2022 · Organizer-related lead · Official-PDF citation only

Jeyakumar/Nirmala/Sarate chapter cited on official PDF page 10; primary chapter retrieval remains pending.

[Primary / author source](https://signalprocessingsociety.org/community-involvement/signal-processing-cup)


### R141 — Non-Contact Pulse Rate Measurement Using Facial Videos (ICADEE)

2020 · Organizer-related lead · Official-PDF citation only

Organizer-associated paper cited on PDF page 10; DOI and primary full text remain pending.

[Primary / author source](https://signalprocessingsociety.org/community-involvement/signal-processing-cup)


### R142 — A Study on Impacts of Ambient Lights and Skin Tone for Contactless Blood Oxygen Measurement using Visible Spectrum Facial Videos

2023 · Organizer-related RGB work · Conference metadata

Arulselvi/Jeyakumar et al.; conference program confirms title; primary paper retrieval remains pending.

[Primary / author source](https://paym.chitkara.edu.in/delcon2023/technical-program.php)


### R143 — Camera oxygenation patent US20230404444A1

2023 application · Adjacent / hardware-dependent · Patent

Prior-art discovery only; not proof that an implementation works or can be reused.

[Primary / author source](https://patents.google.com/patent/US20230404444A1/en)


### R144 — Full-Body Cardiovascular Sensing with Remote Photoplethysmography

2023 preprint · Adjacent: body video · Preprint

Related non-contact sensing; inspect face-only compatibility before reuse.

[Primary / author source](https://arxiv.org/abs/2303.09638)


### R145 — Camera PPG waveforms at the forehead

2023 preprint · Adjacent clinical setup · Preprint

Special clinical capture context; not assumed compatible with ordinary-webcam constraints.

[Primary / author source](https://arxiv.org/abs/2306.09879/)


### R146 — egoPPG

See author repo · Adjacent: egocentric camera · Paper + code lead

Alternative camera geometry; valuable robustness reference, not a standard frontal-face baseline.

[Primary / author source](https://github.com/eth-siplab/egoPPG)


### R147 — CogPhys

See author repo · RGB-compatible research · Paper + code lead

Cognitive-task physiology and evaluation folds; inspect released modalities/labels before use.

[Primary / author source](https://github.com/AnirudhBHarish/CogPhys)


### R148 — Skin-Tone-Invariant Topological Signal Processing: A Framework for Bias-Reducing Optical Measurement Systems

2026 preprint · Fairness research lead · Preprint

New bias-reduction idea; not peer-reviewed validation or a reproduced improvement here.

[Primary / author source](https://www.medrxiv.org/content/10.64898/2026.08.01.26359472v1)


### R149 — rePPG: Relighting Photoplethysmography Signal to Video

2026 · Synthetic augmentation · Paper

Signal-preserving relighting lead; synthetic performance must be checked against real low-light data.

[Primary / author source](https://pmc.ncbi.nlm.nih.gov/articles/PMC13114229/)


### R150 — Performance analysis of remote photoplethysmography deep filtering using LSTM neural network

2022 · Direct RGB · Paper

Post-extraction filtering; compare waveform fidelity as well as HR.

[Primary / author source](https://pmc.ncbi.nlm.nih.gov/articles/PMC9487135/)


## Foundations and classical signal processing


### R151 — Enhancing rPPG pulse-signal recovery by facial sampling and PSD Clustering (CircleClustering)

2025 · Direct RGB · Paper

Corrected title from the chat. Adaptive facial patches and PSD clustering; useful quality-selection candidate, not a guaranteed best tracker.

[Primary / author source](https://expertise.unimi.it/resource/item/1390792?language=en_US) · [Code / related source](https://air.unimi.it/retrieve/handle/2434/1121060/2596995/1-s2.0-S1746809424012163-main.pdf)


## Robustness, fairness and deployment studies


### R152 — SkinMap: Weighted Full-Body Skin Segmentation for Robust Remote Photoplethysmography

2025 preprint · Facial subset only · Preprint

Weighted segmentation can inform ROI selection; full-body input is not the facial-only solution. Avoid unrelated dermatology SkinMap repositories.

[Primary / author source](https://arxiv.org/abs/2510.05296)


## Neural HR and waveform estimation


### R153 — CHROM-Y: Illumination-Adaptive Robust Remote Photoplethysmography Through 2D Chrominance–Luminance Fusion and Convolutional Neural Networks

2025 · Direct RGB · Paper

Luminance/chrominance featurization with CNNs; illumination-dependent generalization must be tested. Not simply a drop-in replacement CHROM equation.

[Primary / author source](https://www.mdpi.com/2624-6120/6/4/72)


### R154 — RADIANT: Better rPPG Estimation Using Signal Embeddings and Transformer

2023 · Direct RGB · Paper

Useful signal-embedding research; not proof that any 24 classical waveforms outperform video models or estimate all three vitals.

[Primary / author source](https://dspace.iiti.ac.in/handle/123456789/11620) · [Code / related source](https://openaccess.thecvf.com/content/WACV2023/papers/Gupta_RADIANT_Better_rPPG_Estimation_Using_Signal_Embeddings_and_Transformer_WACV_2023_paper.pdf)


## Robustness, fairness and deployment studies


### R155 — Assessment of Deep Learning-based Heart Rate Estimation using Remote Photoplethysmography under Different Illuminations

2021 preprint / revised 2022 · Direct RGB · Paper

Compares classical methods and DeepPhys/rPPGNet/PhysNet under illumination changes; findings do not establish universal DSP superiority.

[Primary / author source](https://arxiv.org/abs/2107.13193)


## Datasets and data access


### R156 — BH-rPPG illumination dataset

2021 paper / revised 2022 · Direct RGB · Dataset lead

Thirty-five subjects and three illumination settings described by authors. Current download endpoint and terms still need checking.

[Primary / author source](https://arxiv.org/abs/2107.13193)


### R157 — SYNC-rPPG dataset associated with SkinMap

2025 preprint · Check facial subset · Dataset lead

New capture dataset described by SkinMap authors; access, reference channels and eligibility remain to be established.

[Primary / author source](https://arxiv.org/html/2510.05296)


## Reviews and field maps


### R158 — Deep learning and remote photoplethysmography powered advancements in contactless physiological measurement

2024 · Multi-vital field map · Review

Broad contactless physiology review, not a ready-to-run three-vital model.

[Primary / author source](https://pmc.ncbi.nlm.nih.gov/articles/PMC11298756/)


## Toolboxes, code and implementation references


### R159 — CoVital SpO2 evaluation toolkit

Community repository · Adjacent / input unconfirmed · Python code

Correct upstream repository. Goals mentioning 2% accuracy are project targets, not demonstrated facial-video accuracy; check capture geometry and calibration.

[Primary / author source](https://github.com/CoVital-Project/Spo2_evaluation)


### R160 — Modified pyVHR + HeartPy + CoVital integration (dhananjay1710)

Community repository · Unvalidated integrated demo · Python code

Fork explicitly combines upstream projects. Keep provenance and inspect each module; do not confuse it with official pyVHR or upstream CoVital.

[Primary / author source](https://github.com/dhananjay1710/pyVHR)


### R161 — OpenCV YuNet / FaceDetectorYN

Current docs · Enabling technology · Official docs

Face detector with sparse landmarks; requires association/re-detection to support tracking. Not an independent dense skin tracker.

[Primary / author source](https://docs.opencv.org/4.x/df/d20/classcv_1_1FaceDetectorYN.html)


### R162 — OpenCV Lucas–Kanade optical-flow tutorial

Current docs · Enabling technology · Official docs

Sparse point tracking/refinement; test drift, masks, motion and re-initialization instead of assuming optical flow removes codec artifacts.

[Primary / author source](https://docs.opencv.org/4.x/d4/dee/tutorial_optical_flow.html)


## Foundations and classical signal processing


### R163 — An advanced detrending method with application to HRV analysis (Tarvainen et al.; smoothness priors)

2002 · Adjacent signal-processing method · Paper

Useful detrending candidate. Originally HRV analysis, not a proof of optimal detrending for RGB rPPG or all vital outputs.

[Primary / author source](https://pubmed.ncbi.nlm.nih.gov/12066885/)


## Toolboxes, code and implementation references


### R164 — SciPy Butterworth filter design (butter)

Current docs · Enabling technology · Official docs

Design with actual sampling rate and stable second-order sections; test passband/phase and edge effects.

[Primary / author source](https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.butter.html)


### R165 — SciPy Chebyshev type-II filter design (cheby2)

Current docs · Enabling technology · Official docs

Candidate filter family; stopband ripple and transition/phase tradeoffs need ablation against Butterworth.

[Primary / author source](https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.cheby2.html)


### R166 — SciPy causal second-order-section filtering (sosfilt)

Current docs · Enabling technology · Official docs

Streaming-capable reference; persist filter state across chunks and report delay.

[Primary / author source](https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.sosfilt.html)


### R167 — SciPy forward-backward SOS filtering (sosfiltfilt)

Current docs · Offline reference only · Official docs

Uses forward and backward passes; distinguish offline zero-phase evaluation from causal live inference.

[Primary / author source](https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.sosfiltfilt.html)


### R168 — SciPy Welch power spectral density estimation

Current docs · Enabling technology · Official docs

Useful HR spectra and candidate agreement analysis; dominant peaks can still be motion harmonics.

[Primary / author source](https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.welch.html)


### R169 — SciPy ShortTimeFFT / STFT

Current docs · Enabling technology · Official docs

Explicit window/hop/frequency axes for temporal spectra. Choose model input layout deliberately.

[Primary / author source](https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.ShortTimeFFT.html)


### R170 — PyWavelets thresholding functions

Current docs · Enabling technology · Official docs

Wavelet denoising candidate; verify pulse amplitude/shape preservation rather than assuming it.

[Primary / author source](https://pywavelets.readthedocs.io/en/latest/ref/thresholding-functions.html)


## Learning, compute and deployment resources


### R171 — An Empirical Evaluation of Generic Convolutional and Recurrent Networks for Sequence Modeling (TCN)

2018 · Adjacent sequence-model reference · Paper

General TCN reference for Track 2; no facial HR/SpO2/BP validation implied.

[Primary / author source](https://arxiv.org/abs/1803.01271)


### R172 — ONNX Runtime mobile deployment documentation

Current docs · Optional deployment · Official docs

Evaluate export/operator support and target-device latency; deployment target has not been selected.

[Primary / author source](https://onnxruntime.ai/docs/tutorials/mobile/)


### R173 — Google LiteRT documentation (TensorFlow Lite ecosystem)

Current docs · Optional deployment · Official docs

Current on-device inference reference; conversion and quantization must be verified on real signals.

[Primary / author source](https://ai.google.dev/edge/litert)


### R174 — Apple Core ML Tools documentation

Current docs · Optional Apple deployment · Official docs

Apple-specific conversion/deployment option; not a selected requirement.

[Primary / author source](https://apple.github.io/coremltools/docs-guides/source/overview-coremltools.html)


### R175 — IEEE SPS Resource Center

Current portal · Learning resource · Official SPS source

Biomedical DSP, image/video and ML lectures; content/access varies. Not the primary archive for challenge-paper proceedings.

[Primary / author source](https://signalprocessingsociety.org/publications-resources/sps-resource-center)


### R176 — IEEE SPS challenge-paper listing

Current portal · Learning resource · Official SPS source

Find earlier challenge work and follow individual paper links; audio challenges are not facial-vitals baselines.

[Primary / author source](https://signalprocessingsociety.org/tags/signal-processing-challenges)


### R177 — MathWorks SP Cup software, training and technical support

2027 page checked · Competition support · Official MathWorks source

Current SP Cup page offers software/training/mentor support through a request form; examples may belong to earlier tasks.

[Primary / author source](https://www.mathworks.com/academia/student-competitions/sp-cup.html)


### R178 — IEEE Signal Processing Mentorship Academy (SigMA)

Current program · Optional mentorship · Official SPS source

Structured research-mentoring program; application/access is not guaranteed or a substitute for faculty supervision.

[Primary / author source](https://signalprocessingsociety.org/community-involvement/signal-processing-mentorship-academy-sigma-program)


### R179 — Google Colab FAQ

Current docs · Optional compute · Official docs

Free accelerators may be available; GPU type/limits fluctuate. No guaranteed T4 or five-minute training time.

[Primary / author source](https://research.google.com/colaboratory/faq.html)


### R180 — Kaggle efficient GPU usage guide

Current docs · Optional compute · Official docs

Quota/hardware depend on availability and account settings; check actual quota and checkpoint jobs.

[Primary / author source](https://www.kaggle.com/docs/efficient-gpu-usage)


## Imported videos — unverified links


### R181 — Imported video: Eulerian Video Magnification overview

Supplied chat · Learning lead only · Unverified YouTube link

Title/URL relationship not independently confirmed: direct fetch failed and exact-ID search found no result. Prefer the original MIT project page.

[Primary / author source](https://www.youtube.com/watch?v=ONZcjs1Pjmk)


### R182 — Imported video: How Webcams Detect Your Heart Rate

Supplied chat · Learning lead only · Unverified YouTube link

Preserved for manual review; title/channel/content not verified. Do not treat this as scientific evidence.

[Primary / author source](https://www.youtube.com/watch?v=vi7-qoj80HA)


### R183 — Imported video: BioniChaos rPPG sandbox lead

Supplied chat · Demo lead only · Unverified YouTube link

Supplied link is a video URL, not a verified simulator URL; availability/content remain unconfirmed.

[Primary / author source](https://www.youtube.com/watch?v=faJ36pM1C6k)


### R184 — Imported video: Eulerian Color Magnification walkthrough

Supplied chat · Learning lead only · Unverified YouTube link

Preserve as a manual-review candidate; video content and implementation correctness not checked.

[Primary / author source](https://www.youtube.com/watch?v=5MeeANBgbGo)


### R185 — Imported video: Real-time rPPG with Gemini and Face Mesh

Supplied chat · Demo lead only · Unverified YouTube link

Demo/AI-assisted coding is not validation; availability and actual implementation not confirmed.

[Primary / author source](https://www.youtube.com/watch?v=JH7R5uCAfzw)


### R186 — Imported video: RADIANT paper presentation

Supplied chat · Learning lead only · Unverified YouTube link

Exact video could not be confirmed. The RADIANT paper itself was identified through primary sources.

[Primary / author source](https://www.youtube.com/watch?v=kJkk1AozxFw)


## Historical SP Cup methods and solutions


### R187 — SP Cup 2015 official problem and results

2015 · Closest previous task; contact PPG · Official competition archive

HR under strong exercise motion. Same target as FaceVitals HR, different sensing setup; does not solve facial SpO2/BP.

[Primary / author source](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2015)


### R188 — IEEE SP Cup 2015 PPG dataset — organizer re-release

2015 data / current re-release · Adjacent: wrist PPG + ACC + ECG · Dataset

Organizer-hosted archive now available. Useful algorithm sandbox; not facial-video training or evidence for three-vital performance. Check actual data rights.

[Primary / author source](https://github.com/zhilinzhang/IEEE-SP-Cup-2015-PPG-Dataset)


### R189 — TROIKA: A General Framework for Heart Rate Monitoring Using Wrist-Type Photoplethysmographic Signals During Intensive Physical Exercise

2014 preprint / 2015 journal · Adjacent: contact PPG · Paper

Denoising, sparse spectral reconstruction and verified peak tracking; useful HR processing blueprint, not a camera front end.

[Primary / author source](https://arxiv.org/abs/1409.5181)


### R190 — JOSS: Photoplethysmography-Based Heart Rate Monitoring in Physical Activities via Joint Sparse Spectrum Reconstruction

2015 · Adjacent: PPG + acceleration · Paper

Joint spectra help identify motion peaks. Any video-derived nuisance substitute needs fresh validation; accelerometers are not RGB input.

[Primary / author source](https://arxiv.org/abs/1503.00688)


### R191 — A New Method for Heart Rate Monitoring During Physical Exercise Using Photoplethysmographic Signals (Schack et al.)

2015 · Adjacent: PPG + acceleration · Paper

Paper by members of the overall winning Darmstadt team; multiple adaptive outputs fused in time-frequency space. Not established as an exact archived contest submission.

[Primary / author source](https://www.eurasip.org/Proceedings/Eusipco/Eusipco2015/papers/1570102009.pdf)


### R192 — Real-Time Robust Heart Rate Estimation From Wrist-Type PPG Signals Using Multiple Reference Adaptive Noise Cancellation (Chowdhury et al.)

2016 online / 2018 issue · Adjacent: PPG + acceleration · Paper + MATLAB code

Multiple cleaned signals and candidate tracking; authors overlap BUET Supersignal. Official overall rank was second, despite repository claim of first algorithm performance.

[Primary / author source](https://pubmed.ncbi.nlm.nih.gov/27893403/) · [Code / related source](https://github.com/SayeedChowdhury/Heart-Rate-Estimation-using-PPG-during-exercise-in-intense-motion-artifacts)


### R193 — HeartBEAT: Heart beat estimation through adaptive tracking

2016 · Adjacent: PPG + acceleration · Paper + MATLAB code

RLS artifact reduction and HR tracking evaluated on SP Cup 2015 recordings; useful available implementation, not verified as finalist submission.

[Primary / author source](https://github.com/olivesgatech/HeartBEAT) · [Code / related source](https://arxiv.org/abs/1810.08554)


### R194 — Measuring Heart Rate During Physical Exercise by Subspace Decomposition and Kalman Smoothing

2017 online / 2018 issue · Adjacent: contact PPG · Paper + MATLAB code

Compare subspace separation and temporal smoothing. Smoothing/look-ahead must be distinguished from causal live performance.

[Primary / author source](https://research.unipd.it/handle/11577/3243240) · [Code / related source](https://github.com/AlessandraGalli/PPG)


### R195 — CARMA: A Robust Motion Artifact Reduction Algorithm for Heart Rate Monitoring from PPG Signals

2015 · Adjacent: PPG + acceleration · Paper

SVD-based nuisance/HR subspaces and adaptive tracking; a candidate idea for motion-aware HR, not direct RGB validation.

[Primary / author source](https://eurasip.org/Proceedings/Eusipco/Eusipco2015/papers/1570096797.pdf)


### R196 — deppG: Nonlinear-type time-frequency analysis for instantaneous HR and respiration

2017 · Adjacent: contact PPG · Paper

De-shape STFT and synchrosqueezing tested on the 2015 cup data; useful harmonic-ambiguity research, not a prior winning submission.

[Primary / author source](https://arxiv.org/abs/1701.02072)


### R197 — PPG-based heart rate estimation using Wiener filter, phase vocoder and Viterbi decoding

2017 · Adjacent; offline decoding · Paper

Temporal path selection across time-frequency states; paper targets offline scenarios. A causal or bounded-delay adaptation must be tested separately.

[Primary / author source](https://cora.ucc.ie/items/c9fde456-94cd-4c90-bc50-3e910cf025e0)


### R198 — SP Cup 2016 — post-competition release and technical specification

2016 · Adjacent: ENF / lighting interference · Official technical document

Weak power-grid signatures in media; useful nuisance-modeling context. Not a pulse estimator; do not blindly notch grid frequencies in frame-sampled RGB traces.

[Primary / author source](https://sigport.org/sites/all/modules/pubdlcnt/pubdlcnt.php?fid=4952)


### R199 — SP Cup 2016 team report: ENF estimation and classification (SigPort fid 899)

2016 · Adjacent: weak periodic signals · Team-report lead

Indexed text discusses Prony/ARMA features and classifiers. Full fetch blocked, so precise implementation and team attribution need confirmation.

[Primary / author source](https://sigport.org/sites/all/modules/pubdlcnt/pubdlcnt.php?fid=899)


### R200 — SP Cup 2017 official real-time beat-tracking specification

2017 · Adjacent: music periodicity · Official technical document

Causal periodicity estimation and embedded demo requirements; music tempo is not cardiac rhythm physiology.

[Primary / author source](https://signalprocessingsociety.org/sites/default/files/uploads/publications_resources/news/ICASSP_2017_SPCup.pdf)


### R201 — Predictive Real-Time Beat Tracking from Music for Embedded Application (RTBT)

2018 paper / 2017 cup · Adjacent: music tracking · Paper + Python code

Author repo reports 2017 honorable mention; inspect predictive timing and embedded design. Python 2.7-era dependencies; no physiological validation.

[Primary / author source](https://github.com/iah3/RTBT)


### R202 — SP Cup beat-tracking code and UMD final-submission report

2017 context · Adjacent: music tracking · Code + team report

Repository includes MATLAB/Python code and a UMD final report. Exact finalist identity/rank not established from this repository alone.

[Primary / author source](https://github.com/nkandpa2/Beat-Tracking)


### R203 — madmom online beat tracking and maintainer streaming discussion

2017 cup ecosystem / maintained code · Adjacent: music tracking · Code + discussion

Inspect online RNN/DBN processing and stream handling; music weights cannot estimate HR. Code and model licenses differ.

[Primary / author source](https://github.com/CPJKU/madmom) · [Code / related source](https://groups.google.com/g/madmom-users/c/yYtp6Y43yWQ/m/5iH_AQXzCQAJ)


### R204 — IEEE TV: SP Cup 2017 finalist presentations

2017 · Presentation / deployment reference · Official presentation collection

Official collection includes finalist talks. Useful report/demo structure; access may require membership. Videos not watched in this pass.

[Primary / author source](https://ieeetv.ieee.org/ondemand/ieee-sp-cup-2017)


### R205 — Application of DenseNet in Camera Model Identification and Post-processing Detection

2018 preprint / 2019 workshop · Adjacent: camera-domain effects · Paper

Uses SP Cup 2018 data; camera/post-processing differences motivate device-separated evaluation. Not an rPPG estimator or verified winning submission.

[Primary / author source](https://arxiv.org/abs/1809.00576) · [Code / related source](https://openaccess.thecvf.com/content_CVPRW_2019/papers/Media%20Forensics/Rafi_Application_of_DenseNet_in_Camera_Model_Identification_and_Post-processing_Detection_CVPRW_2019_paper.pdf)


### R206 — DFCon: Attention-Driven Supervised Contrastive Learning for Robust Deepfake Detection

2025 · Adjacent: facial image generalization · Team solution paper

Explicit 2025 SP Cup report; useful domain-generalization reading. Image classification cannot recover pulse timing or validate BP/SpO2.

[Primary / author source](https://arxiv.org/abs/2501.16704) · [Code / related source](https://souvikghosh.netlify.app/post/sp-cup/)


### R207 — SP Cup 2026 SuperZooooom winner — implementation summary

2026 · Adjacent: edge / system engineering · Sponsor implementation account

MATLAB DSP/simulation combined with PyTorch models and smartphone deployment. Useful integration precedent; not reusable vitals weights or complete released code.

[Primary / author source](https://www.mathworks.com/academia/students/competitions/global-competitions/winners.html) · [Code / related source](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2026)


### R208 — Adaptive physiology-informed correction for reliable remote photoplethysmography heart-rate monitoring

2026 · Direct RGB HR bridge · Paper

Modern rPPG estimate-correction study cites older wrist-PPG tracking work. Useful bridge to temporal HR validation; test response lag and retained failures, not just smoothness.

[Primary / author source](https://pmc.ncbi.nlm.nih.gov/articles/PMC13000236/)
