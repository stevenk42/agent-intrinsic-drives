## Modular Intrinsic-Reward Drives

Curiosity   (reward for uncertainty reduction):
    ΔU = ΔH × (1 + k_T · T)

Boredom     (penalty for repetition):
    M_bore = Σ z²

Pair-Bonding (reward for mutual information with a partner):
    M_pair = I(s₁ ; s₂)

Resource Competition (sparsity pressure):
    L_total = Σ_μ L  +  β ‖C − D(E(C))‖²

Self-Model  (coherence of internal code):
    L_recon = ‖C − D(E(C))‖² × (1 + k′_T · T)

Anxiety     (penalty for excessive uncertainty):
    M_anx = 𝟙 [ H[q] > τ ]
    
Reputation  (reward/penalty from social standing):
    M_rep = −Σ_R ⟨j | ρ | j⟩

Costly Signaling (cost for visible signals):
    M_signal = Σ_c P

Fairness    (minimise group inequity):
    M_fair = −Var(U)

Altruism    (reward for others’ gain):
    M_altruism = Σ_w ΔU

Playfulness (reward for surprise):
    M_play = 𝔼[Surprise] × (1 + k″_T · T)

Legacy      (reward for persistence of impact):
    M_legacy = 𝔼[Persistence]

Adaptation  (reward for policy flexibility):
    M_adapt = −Σ ‖Δπ(e)‖²

Mystery     (reward for others’ uncertainty):
    M_mystery = H(z | O)

Self-Ontology (time-aware doubt about “simulation vs emulation” status):
    M_ont,t = ṼΔH_t × (1 + k_T^{ont} · t) − λ_prem · 𝟙 [ H[p_t] < τ_prem ]

        where   ṼΔH_t = Σ_{τ=1}^{t} e^{−α(t−τ)} ( H[p_{τ−1}] − H[p_τ] )

Fear (amplifies curiosity at boundaries):
M_fear = (1 + α_fear · F) × ΔU

Edge-Seeking (reward for encountering operational/epistemic boundaries):
M_edge = 𝟙[at boundary] × γ_edge × (ΔH + ΔR)
