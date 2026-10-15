# Past IEEE SP Cups: relevance to FaceVitals 2027

Checked **15 October 2026**. Scope: all **13 previous SP Cup editions listed in the official archive, 2014–2026**. SP Cup is distinct from VIP Cup and other SPS challenges.

## Answer

**2015 is the closest technical predecessor:** optical heart-rate estimation under strong motion contamination. The other useful connections are 2017 (real-time periodicity tracking), 2016 (weak signatures and lighting-related nuisance), 2018 (camera-processing/device differences), and 2026 (real-time target isolation and edge integration).

No earlier archived task reviewed here combined RGB facial-video HR, SpO2 and blood pressure. The useful inheritance is a set of methods and engineering practices, not a previously solved FaceVitals system.

## What was actually checked

Reviewed the official year-specific problem descriptions for 2014–2026, resolved a broken/mislabeled 2025 archive link using the official 2025 PDF, and followed relevant technical specifications, papers, code and discussions. This is not a claim that every historical PDF, private submission, forum post or repository was recovered. Coverage and access limitations are explicit below. No code was executed, data downloaded or performance independently reproduced.

Primary starting point: [official past-cup index](https://signalprocessingsociety.org/community-involvement/signal-processing-cup). The year coverage is also available as [JSON](Year_by_Year_Coverage.json).

## Every archived year

| Year | Problem | Relevance to FaceVitals | Source coverage |
|---|---|---|---|
| [2014](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2014) | Image restoration / super-resolution for single-particle analysis | Low: image restoration concepts; different imaging domain. | Official SPS problem description reviewed; original conference link is historical. |
| [2015](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2015) | Heart rate monitoring during physical exercise using wrist-type PPG signals | Highest: optical pulse extraction, strong motion interference and HR tracking. | Official SPS description/results, organizer data repo and related methods reviewed. Original detailed-task link failed. |
| [2016](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2016) | Exploring power signatures for location forensics of media recordings | Moderate: weak periodic signal extraction and lighting interference. | Official description and post-competition specification located; several SigPort report fetches blocked. |
| [2017](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2017) | Real-time beat tracking challenge | Moderate: causal periodicity tracking, ambiguity and embedded latency. | Official description and technical PDF reviewed; team code and official presentation collection located. |
| [2018](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2018) | Forensic camera model identification | Moderate: camera-processing signatures and device generalization. | Official description reviewed; detailed-document link redirected to the current cup. Related author paper located. |
| [2019](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2019) | Search and rescue with drone-embedded sound-source localization | Low: signal separation under interference; different modality. | Official problem description and organizer overview located. |
| [2020](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2020) | Unsupervised abnormality detection using intelligent heterogeneous autonomous systems | Low: system-level validation and failure handling; different task. | Official description and winning-team interview reviewed. |
| [2021](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2021) | Configuring an intelligent reflecting surface for wireless communications | Very low: no physiological or facial-video task overlap. | Official description and organizer repository located. |
| [2022](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2022) | Synthetic speech attribution | Very low: generalization lessons only; audio forensics. | Official problem description reviewed. |
| [2023](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2023) | Psychosis classification from resting-state fMRI | Low: biomedical study-design context; different signal and target. | Official problem description/results reviewed; no facial-vitals solution identified. |
| [2024](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2024) | ROBOVOX: far-field speaker recognition by a mobile robot | Low: robustness and multi-channel modeling; different modality. | Official problem description and system-description paper located. |
| [2025](https://signalprocessingsociety.org/sites/default/files/uploads/community_involvement/docs/2025_spcup_official_doc.pdf) | DFWild-Cup: deepfake face detection in the wild | Limited: facial image/domain-shift evaluation, not pulse recovery. | Verified official 2025 PDF and DFCon paper; archive link ending 2025-0 incorrectly displays 2024 content. |
| [2026](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2026) | AV Zoom: real-time audio-visual zooming on smartphones | Moderate: target isolation, live integration and compute budgeting. | Official problem description/document and winner implementation summary located. |

## 2015: the useful predecessor

The [official task/results](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2015) concern exercise-contaminated wrist PPG. The final overall winner was Signal Processing Crew Darmstadt; BUET Supersignal placed second. This ranking should not be confused with a code author's claim of best algorithm-only performance.

Why we should read it: recovering a weak optical pulse when motion creates competing periodic peaks is close to our HR difficulty. Why we cannot copy it unchanged: wrist PPG has controlled sensor illumination and the methods often use simultaneously measured acceleration. Facial RGB has different optics, motion and compression; external acceleration must not silently enter our RGB inference pipeline. This lineage provides no facial SpO2/BP labels or validation.

### Highest-value papers/code

1. **Schack/Sledz/Muma/Zoubir, EUSIPCO 2015.** The [paper](https://www.eurasip.org/Proceedings/Eusipco/Eusipco2015/papers/1570102009.pdf), by members of the overall winning team, uses two PPG channels and three acceleration axes, forms six adaptive-filter outputs and combines them for HR tracking. It is particularly relevant to the idea of multiple candidate signals. It does not justify an arbitrary 24-channel ensemble, and we did not recover an exact final-submission code release.
2. **Chowdhury et al., multiple-reference adaptive noise cancellation.** [Paper](https://pubmed.ncbi.nlm.nih.gov/27893403/) and [author MATLAB code](https://github.com/SayeedChowdhury/Heart-Rate-Estimation-using-PPG-during-exercise-in-intense-motion-artifacts). Study how several cleaned signals generate plausible HR candidates and how continuity resolves ambiguity. The previous HR estimate can help, but an incorrect track can also persist. These are wrist-sensor results.
3. **TROIKA.** [Primary paper](https://arxiv.org/abs/1409.5181). Decomposition, sparse spectrum reconstruction and checked peak tracking give a clear modular alternative to simply taking the largest FFT peak. This is an influential benchmark framework associated with the dataset, not the official overall winning team solution.
4. **JOSS.** [Primary paper](https://arxiv.org/abs/1503.00688). Joint sparse spectral estimation of pulse and acceleration helps distinguish motion-related peaks. Transfer would require testing whether nuisance signals extracted from our video satisfy useful assumptions.
5. **HeartBEAT.** [Lab code and paper links](https://github.com/olivesgatech/HeartBEAT). Available MATLAB implementation of adaptive filtering and tracking evaluated on cup recordings. It is a later dataset-based method, not verified as a cup finalist submission.
6. **Subspace decomposition and Kalman smoothing.** [Author code](https://github.com/AlessandraGalli/PPG), [institutional paper record](https://research.unipd.it/handle/11577/3243240). Useful for separating subspaces and comparing temporal stabilization. Explicitly distinguish filtering from smoothing and report any future-data dependence.
7. **Further alternatives:** [CARMA](https://eurasip.org/Proceedings/Eusipco/Eusipco2015/papers/1570096797.pdf), [deppG](https://arxiv.org/abs/1701.02072), and [Wiener filtering / phase vocoder / Viterbi decoding](https://cora.ucc.ie/items/c9fde456-94cd-4c90-bc50-3e910cf025e0). The last paper explicitly targets offline use; copying its decoding wholesale would not establish causal live operation.

### Dataset recovered

The organizer has an accessible [GitHub re-release](https://github.com/zhilinzhang/IEEE-SP-Cup-2015-PPG-Dataset), including competition archives, reference BPM files and associated papers. This can support a small pulse-processing exercise. It cannot replace a paired facial-video dataset. Inspect actual files, timestamps, subject/recording identity and rights before using it; do not mistake the number of recordings for distinct subjects.

## 2017: real-time periodicity tracking

The [official technical specification](https://signalprocessingsociety.org/sites/default/files/uploads/publications_resources/news/ICASSP_2017_SPCup.pdf) concerns musical beats on embedded systems. Its relevance is algorithm structure: online processing, evolving rhythm, timing ambiguity and latency. Musical tempo priors and learned music weights are not cardiac physiology.

- [RTBT author code](https://github.com/iah3/RTBT): predictive embedded music tracking; repository reports a 2017 honorable mention. Dependencies are Python 2.7-era and need assessment before reproduction.
- [UMD final-report/code repository](https://github.com/nkandpa2/Beat-Tracking): concrete report and MATLAB/Python implementation to inspect; exact finalist identity/rank not established by the repo alone.
- [madmom](https://github.com/CPJKU/madmom): inspect online RNN/DBN processing and the [maintainer streaming discussion](https://groups.google.com/g/madmom-users/c/yYtp6Y43yWQ/m/5iH_AQXzCQAJ). Source-code and model licenses differ; do not assume all weights can be reused under the source license.
- [Official IEEE TV finalist talks](https://ieeetv.ieee.org/ondemand/ieee-sp-cup-2017): examples of report/demo communication. Collection identified; talks not watched in this pass.

**Transfer hypothesis:** track a distribution or several candidate pulse frequencies over successive windows instead of independently choosing one peak. Compare against a simpler implementation and assess lag during changing HR.

## 2016: lighting and weak-signal extraction

[Official task](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2016), [post-competition specification](https://sigport.org/sites/all/modules/pubdlcnt/pubdlcnt.php?fid=4952) and [team-report lead](https://sigport.org/sites/all/modules/pubdlcnt/pubdlcnt.php?fid=899).

The objective was identifying recording location from electric-network-frequency signatures embedded in media. For FaceVitals, the useful inference is that camera intensity can contain structured periodic nuisance signals besides the pulse. The indexed team report discusses parametric spectral features and classification, but a blocked full fetch prevents endorsing its exact implementation.

Do not apply a 50/60-Hz notch blindly to frame-sampled facial traces: the relevant observable interference depends on lighting, exposure/readout and sampling/aliasing. Treat illumination assessment as a separate experiment, and validate that suppression preserves the pulse.

## 2018: device and post-processing differences

[Official task](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2018) and a [dataset-based DenseNet paper](https://arxiv.org/abs/1809.00576) show that images retain camera/post-processing signatures. Our engineering inference is to test whether HR estimators rely on device artifacts or remain accurate across held-out cameras, resolutions and codecs. Camera identification accuracy is not pulse accuracy. No need to add a camera classifier simply because this competition exists.

## 2025: face imagery, but a different prediction target

The [official PDF](https://signalprocessingsociety.org/sites/default/files/uploads/community_involvement/docs/2025_spcup_official_doc.pdf) confirms real/fake **image** discrimination, including unseen generation methods and source datasets. [DFCon](https://arxiv.org/abs/2501.16704) is a genuine task-specific solution paper. Its relevance is handling domain variation; it is not an rPPG/BP architecture. A single still image does not contain the pulse-time sequence our task needs.

An archive entry [ending in `2025-0`](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2025-0) currently contains 2024 ROBOVOX text. We used the actual 2025 document to resolve that mismatch. Also avoid the unrelated time-series forecasting paper sharing the name DFCon.

## 2026: system integration rather than physiological inference

[Official task](https://signalprocessingsociety.org/community-involvement/ieee-signal-processing-cup-2026) covers smartphone AV zoom and selected-target isolation. The [MathWorks winner account](https://www.mathworks.com/academia/students/competitions/global-competitions/winners.html) describes SuperZooooom combining MATLAB simulation/DSP with PyTorch models and smartphone deployment. It is a useful example of developing a complete hybrid system; it does not establish a mandatory smartphone target for 2027. A complete public winner code repository was not found in this pass.

## A direct modern bridge back to facial rPPG

[Adaptive physiology-informed correction for reliable rPPG HR monitoring (2026)](https://pmc.ncbi.nlm.nih.gov/articles/PMC13000236/) studies correction of HR estimates and cites older PPG tracking work. It is a useful companion to the 2015 lineage because it applies estimate-level correction in the camera setting. It is not an old cup submission. Check coverage, initialization and response delay; smoother output alone is not proof of accuracy.

## What to try next — proposals, not measured improvements

| Question | Small experiment | Main risk |
|---|---|---|
| Do temporal candidates beat a largest-peak baseline? | Same RGB extraction and HR windows; compare independent peak selection with confidence-aware multi-candidate tracking | Locking onto a motion harmonic; lag during real HR changes |
| Can video motion act as a nuisance reference? | Extract eligible landmark/optical-flow motion from the same video; compare filtering with and without that reference | Motion cue is not wrist acceleration; may correlate with desired physiology |
| Does fusion add useful diversity? | Compare best single POS/CHROM output, simple quality gating and selected fusion | Many equally wrong/correlated channels; test-set tuning |
| Do illumination artifacts explain failures? | Compare performance across available lighting conditions; inspect raw regional spectra/timestamps | Aliasing and exposure effects; removing actual physiology |
| Does the approach generalize across devices? | Hold out subjects and, where possible, an entire camera/device domain | Small groups or leakage through near-duplicate recordings |

Keep HR trajectories, rejected windows, output coverage, runtime and failure examples. Preserve raw RGB/DC information for future SpO2/BP work. These experiments must use facial-video ground truth before making any FaceVitals performance claim.

## Recommended reading order for this historical branch

1. 2015 Darmstadt method paper and BUET paper/code.
2. TROIKA and JOSS for decomposition/spectrum/tracking alternatives.
3. HeartBEAT or Galli implementation for a practical MATLAB study.
4. The 2026 facial-rPPG correction paper as a bridge to our actual modality.
5. 2017 online tracking material only if temporal decoding becomes a bottleneck.
6. 2016/2018/2026 material selectively for illumination, device testing or deployment.

This is a side branch of the main reading plan. Continue facial RGB baselines and subject-separated evaluation; the historical contact-PPG data should not consume the whole team's preparation time.

## Access / evidence limits

Original full technical statements were not all recoverable. Several legacy pages route to the current competition, some detailed material lives on Piazza/SigPort, and video membership access was not exercised. Official year descriptions establish task topics; a later paper using cup data is not automatically a team submission or winning solution. Public code was located and inspected at README/file-list level, not executed. No claim of exhaustive recovery of every team solution is made.

The updated main catalogue lists the newly located papers, code, technical documents and presentation sources in a separate **Historical SP Cup methods and solutions** category. Existing resource IDs remain stable. 
