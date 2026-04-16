# DS-Design-Principle
## Dimensional Shift Design Principle (Project D-Link)

**Open-source reference implementation and research artifacts**

This repository accompanies the scientific preprint:

> **Dimensional Shift Design Principle (Project D-Link):  
> A Policy-Driven Architecture for Heterogeneous CPU–GPU–Quantum Computation**

The project introduces a **policy-driven, dimension-oriented computational architecture**
designed to unify heterogeneous execution substrates including classical CPUs,
GPUs (CUDA), and quantum backends.

---

## 📄 Research Paper

- **Preprint (ResearchGate DOI):**  
  https://doi.org/10.13140/RG.2.2.32197.72168

- **License (paper/manuscripts):**  
  Creative Commons Attribution 4.0 (CC BY 4.0)

---

## 🧠 Core Idea

The **Dimensional Shift Design Principle** models computation as adaptive routing
and transformation of **dimensional states** over a central **Dimension Bus**.

Each dimensional state encapsulates:
- data payload
- metadata
- transformation lineage
- policy constraints
- multi-objective scoring vector

Execution is performed across **semi-autonomous computational colonies**
(acquisition, detection, control, meta-control, quantum-policy),
which communicate exclusively via the Dimension Bus.

This enables:
- runtime reconfiguration
- loose coupling and fault isolation
- replayability and traceability
- hybrid classical–GPU–quantum workflows

---

## 🧩 Formal Model (Summary)

A dimensional state is defined as:

D = (S, M, T, P, Σ)

csharp
Zkopírovat kód

with global state space:

𝓓 = 𝓢 × 𝓜 × 𝓣 × 𝓟 × ℝ^k

yaml
Zkopírovat kód

Policies optimize expected utility over dimensional trajectories under
resource constraints, latency bounds, and information-theoretic objectives.

---

## 🚀 Applications

- heterogeneous and adaptive computing systems
- cyber-physical control architectures
- GPU-accelerated optimization pipelines
- hybrid quantum–classical workflows
- experimental computing architectures

---

## 🔮 Future Work

Planned research directions include:
- autonomous policy learning (reinforcement learning)
- formal verification of dimensional invariants
- FPGA-based implementations of the Dimension Bus
- large-scale distributed deployments
- deeper integration with near-term quantum hardware
- standardized open interfaces for dimensional execution

---

## 📦 Repository Contents

- Research manuscripts (PDF / DOCX)
- Archived academic materials
- Release artifacts corresponding to public disclosures

See **GitHub Releases** for versioned, timestamped disclosures.

---

## 🏷 Versioning & Integrity

- **Current release:** `v1.0.0 — Initial public disclosure`
- **Release tag:** v1.0.0
- **Integrity:** cryptographic checksums are referenced via `CHECKSUMS.sha256`
  (to be finalized)

---

## 📜 Licensing

- **Code:** Apache License 2.0  
- **Manuscripts / PDFs:** CC BY 4.0  

See `LICENSE` and `NOTICE` for details.

---

## 📖 How to Cite (IEEE)

> J. Burda, J. Havlasek “Dimensional Shift Design Principle (Project D-Link Qywaria made):  
> A Policy-Driven Architecture for Heterogeneous CPU–GPU–Quantum Computation,”  
> *ResearchGate Preprint*, Jan. 2026,  
> doi: 10.13140/RG.2.2.32197.72168.

---

Grok Analysis of the project:

Toto je velmi zajímavý a komplexní ZIP balíček! Obsahuje Dimensional Shift (PST) Prototype v2.6.0 – modulární referenční architekturu a prototyp, který kombinuje:

Pulse-Space Transduction (PST) pro převod analogových signálů (např. 0–230 V) na multi-dimenzionální pulzní/bitové proudy.
Heartbeat-like rhythm (Expand/Yang ↔ Collision/Yin, neboli Dimensional Expansion – DE vs. Dimensional Reduction/“Dim-plosion” – DR).
Hierarchii kolonií (organism-of-organisms): ADC → Detection → Control → Meta (s adaptací konfigurace v reálném čase, včetně birth/kill dimenzí a breath controlu).
D-Link – univerzální bridge/co-processor pro role jako insight evaluation, Top-K selection a gate/breath optimization, s podporou CPU / CUDA (CuPy) a připraveností na QPU (simulátor, Cirq, Google Quantum Engine skeleton).
CUDA primitivy (UTB-style: vector add, matmul global, conv2D RGB se shared memory) zabalené do DS-pulzu pro autotuning launch parametrů.
Dynamic 10D optimizer s polygon/radar grafy, baselines a GPU/CPU benchmarky.
Reproducible artefakty: CSV datasety, ploty, PDF reporty, markdowny, QPU job logging + replay atd.

Rychlý přehled struktury (z README + FINAL_README)

Hlavní namespace: pst/ (dimension_bus, router, colonies, config bundles, decoder, organism_runtime atd.).
Demos (doporučené pořadí):
python -m pst.sim_harness
python examples/run_pst_adc_pipeline_cfg.py (config-driven PST-ADC)
python examples/run_colony_stack.py
python examples/run_dimensional_shift_live.py (live breath + dim birth/kill + cfg rollover)
D-Link: run_dlink_quantum_bridge_sim.py, run_dimensional_shift_live_qpu.py, CUDA varianty atd.
Teacher/Presentation mode: examples/presentation_mode_teacher_demo.py (vygeneruje PDF + talk-track).
Dynamic 10D: examples/demo_ds_dynamic_10d_gpu_vs_baselines.py
UTB CUDA: apps/cuda_primitives_dlink/ + benchmark_suite.sh

Docs: Velmi detailní (01_architecture_overview.md až 27_dlink_scaling_benchmark.md) + Project D-Link/ (pseudokód, filosofie, signed statement od Bc. Jiřího Burdy FAI UTB).
Verze 2.6.0: Přejmenování na Project D-Link, one-command export (scripts/export_all.sh), report summarizer.

Projekt je koncipován jako robustní, replayable a multi-backend systém – všechny rozhodnutí (Top-K, breath, cfg) jdou přes D-Link, logují se do bus packetů/QPU jobů a dají se replayovat. Filozoficky spojuje klasické computing, GPU akceleraci a koncepty inspirované kvantovým (ale zůstává klasické).
Co bys rád dělal dál?

Spustit konkrétní demo a popsat výstup/ploty? (Můžu ti poradit s env vars, očekávanými výsledky nebo troubleshootovat.)
Analyzovat část kódu (např. organism_runtime.py, ds_lite.py, D-Link selector, conv2D shared vs global)?
Vysvětlit koncept (např. jak funguje Expand vs Collapse, proč je to užitečné pro waveform reconstruction + anomaly detection, nebo mapping na QPU role)?
Porovnat s podobnými paradigmaty (hyperdimensional computing, predictive coding, pulse-based/neuromorphic systémy)?
Nápady na rozšíření (např. integrace s real hardware, lepší QPU mapping, GUI benchmark button, nebo aplikace na jiné signály než voltage)?
Generovat vizualizace (např. radar polygon z 10D parametrů, nebo úpravu existujících plotů)?
Nebo něco úplně jiného – třeba shrnutí pro prezentaci, nebo jak to prezentovat učiteli/na UTB?

Řekni mi, co tě na tom nejvíc zajímá nebo co chceš vyzkoušet – rád pomůžu prozkoumat, spustit, vysvětlit nebo vylepšit! 🚀2,2sRychlýVysvětli D-Link QPU roleD-Link QPU role jsou tři klíčové „úlohy“ (roles), které D-Link Quantum Bridge poskytuje v rámci architektury Dimensional Shift (DS / PST).
D-Link funguje jako univerzální co-processor bridge mezi hlavním systémem (Linux/Python runtime s Dimension Bus) a akcelerátorem – v tuto chvíli primárně simulátorem, případně CUDA/GPU nebo budoucím skutečným QPU (Google Quantum Engine skeleton + Cirq).
Proč vůbec QPU role existují?
Dimensional Shift pracuje v pulzním rytmu (heartbeat):

Expand fáze (Yang / DE – Dimensional Expansion) → systém otevírá mnoho dimenzí/lanes, zkouší nové projekce, více explorace.
Collision fáze (Yin / DR – Dim-plosion) → komprimuje, vybírá nejlepší dimenze (Top-K), upravuje parametry, prune slabé lanes.

Tyto rozhodnutí (které dimenze přežijí, jak nastavit breath Te/Tc, jak ohodnotit užitečnost dimenze) jsou výpočetně náročné, pokud je dimenzí hodně (tisíce až miliony). Proto D-Link nabízí tři specializované role, které lze delegovat na rychlý backend (CPU → CUDA → případně QPU).
Tři QPU role (přesně jak jsou definovány v prototypu)

Top-K selector (topk_subset)
Účel: Během collision fáze vybere subset nejlepších dimenzí (Dim-plosion / Dimensional Reduction).
Vstup: Seznam kandidátních dimenzí + jejich skóre (insight scores) nebo priory.
Výstup: Seznam ID dimenzí, které se mají zachovat (velikost K).
Jak to pomáhá DS: Místo aby systém držel všechny dimenze pořád, prudce sníží počet aktivních lanes na ty nejužitečnější → šetří výpočetní zdroje a zvyšuje robustnost.
Backend mapping: Na QPU/simulátoru se dá realizovat jako subset sampling (např. state-preparation + measurement).

Gate schedule / Breath optimizer (gate_opt)
Účel: Optimalizuje „dech“ systému – poměr expand vs. collision (parametry Te = expand time, Tc = collision time).
Vstup: Aktuální Te/Tc, constraints (min/max), proxy objektivu (např. pain = rekonstrukční chyba nebo anomálie), případně learning progress.
Výstup: Nové hodnoty Te/Tc a případně jemné úpravy gate na jednotlivých dimenzích.
Jak to pomáhá DS: Systém se adaptivně „dýchá“ – při vysokém „pain“ (např. velká chyba nebo nebezpečný napěťový stav) se více zaměřuje na collision (rychlejší komprese a kontrola). Při dobrém stavu více exploruje (delší expand).
Backend mapping: Optimalizační úloha – na QPU lze mapovat jako parametrický search nebo variational-like obvod.

Insight evaluator (insight_eval)
Účel: Ohodnotí „užitečnost“ každé dimenze (stochastic scoring).
Vstup: Feature summary z routeru (mean, std, count ones atd.), rekonstrukční chyby, anomaly signály, případně history.
Výstup: Skóre pro každou dimenzi (insight score) – vyšší = důležitější dimenze.
Jak to pomáhá DS: Poskytuje data pro Top-K filtr a pro rozhodnutí o birth/kill dimenzí v meta kolonii. Bez dobrého insight by byl výběr slepý.
Backend mapping: Stochastic scoring – na QPU simulátoru se realizuje přes sampling z připravené distribuce.


Jak to celé funguje v praxi (D-Link flow)

Hlavní DS runtime (colony hierarchy, router, meta colony) emituje problem descriptor (JSON-like struktura popisující, kterou roli chce spustit + vstupní data).
D-Link platform selector (DLINK_PLATFORM = cpu | cuda | qpu-sim | qpu-cirq | qpu-engine) rozhodne, kam úlohu pošle.
Výsledek se vždy vrací jako Dimension Bus packet (insight, cfg intent atd.) → vše je replayovatelné.
Existuje LoggingSampler → všechny QPU volání se logují do JSONL (runs/qpu_jobs.log) a dají se replayovat i bez reálného hardwaru.
V současné verzi (v2.6.0) je default simulátor (čistý Python + numpy), volitelně Cirq, skeleton pro Google Quantum Engine.

Proč je to navrženo „QPU-ready“, i když QPU ještě není?

Stejný problem descriptor rozhraní funguje pro všechny backendy.
Role jsou navrženy tak, aby byly mapovatelné na kvantové primitivy (sampling, variational optimization, subset selection).
Systém zůstává plně funkční i bez QPU – jen se přepne na CPU/CUDA.
Budoucí rozšíření: reálné QPU by mohlo poskytnout lepší sampling nebo rychlejší optimalizaci v extrémně vysokých dimenzích.

Shrnutí v jedné větě
D-Link QPU role jsou tři specializované akcelerační funkce (insight_eval, topk_subset, gate_opt), které umožňují Dimensional Shift systému inteligentně řídit svůj „dech“ a počet dimenzí tím, že deleguje klíčová rozhodnutí na rychlý co-processor (dnes CUDA/simulátor, zítra potenciálně reálné QPU).
------------------------------------------------------------------------------------------------------------------------------------------

## 🤝 Status

This repository represents an **open, timestamped public disclosure**.
The work is **not yet peer reviewed**.

Feedback, discussion, and collaboration are welcome.
