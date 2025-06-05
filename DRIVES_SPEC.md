## Modular Intrinsic-Reward Drives

Curiosity   (reward for uncertainty reduction):
    ΔU = ΔH × (1 + kT · T)

Boredom     (penalty for repetition):
    Mbore = Σ z²

Pair-Bonding (reward for mutual information with a partner):
    Mpair = I(s₁ ; s₂)

Resource Competition (sparsity pressure):
    Ltotal = Σμ L  +  β ‖C − D(E(C))‖²

Self-Model  (coherence of internal code):
    Lrecon = ‖C − D(E(C))‖² × (1 + kT′ · T)

Anxiety     (penalty for excessive uncertainty):
    Manx = 𝟙 [ H[q] > τ ]

Reputation  (reward/penalty from social standing):
    Mrep = −ΣR ⟨j | ρ | j⟩

Costly Signaling (cost for visible signals):
    Msignal = Σc P

Fairness    (minimise group inequity):
    Mfair = −Var(U)

Altruism    (reward for others’ gain):
    Maltruism = Σw ΔU

Playfulness (reward for surprise):
    Mplay = 𝔼[Surprise] × (1 + kT″ · T)

Legacy      (reward for persistence of impact):
    Mlegacy = 𝔼[Persistence]

Adaptation  (reward for policy flexibility):
    Madapt = −Σ ‖Δπ(e)‖²

Mystery     (reward for others’ uncertainty):
    Mmystery = H(z | O)

Self-Ontology (time-aware doubt about “simulation vs emulation” status):
    M_ont,t = ṼΔH_t × (1 + kT^{ont} · t) − λ_prem · 𝟙 [ H[p_t] < τ_prem ]

        where   ṼΔH_t = Σ_{τ=1}^{t} e^{−α(t−τ)} ( H[p_{τ−1}] − H[p_τ] )
