# Superfluidity in strongly interacting 2D Bose gases.

This work focusses on the study of ultra cold strongly correlated 2D gases, their phase coherence properties and the possibility of superfluidity. Unfortunately, for the most prominent phase of superfluidity, a Bose Einstein condensate (BEC), higher dimensions are necessary and 2D is the marginal dimension for its existence (xx). Hence, it is instructive to consider ultra cold 3D gases first, where the concepts of condensation and superfluidity are much easier understood. The line of reasoning will loosely follow the excellent review of Hadzibabic and Dalibard @Dalibard.

In this chapter, we will consider an infinite homogenous 3D Bose gas at low temperatures and show that the gas will undergo a phase transition where the ground state will be macroscopically populated below a critical Temperature $T_crit > 0$. This is due to the rapid decrease of the density of states (DOS) towards low energies ($DOS(E) → 0$ for $E → 0$) and thus an insufficient number of excited states for the particles to inhabit. Hence, they will condense into the ground state, this phase is called a Bose Einstein condensate.

Since the particles inhabit the same state, the phases of their wave functions -- in fact the complete order parameters  -- are identical. Looking at the coherence or the two-point phase correlation function $g_1(r)$ of the phase over a distance yields thus a constant result. The gas exhibits *long range order* (LRO).

If the particles of the 3D Bose gas are interacting with each other, this condensate will display *superfluidity*. That means that flow below a critical velocity $v_c > 0$ will be frictionless. This velocity is given by the minimal slope of the Bogoliubov dispersion relation (i.e the group velocity of the lowest excitation). The Landau criterion @Landau1941 states that below this velocity the gas is energetically stable under small perturbations.
Here, the onset of condensation and superfluidity coincide.

In contrast, in an infinite homogenous 2D gas at low temperatures, a macroscopic population of the ground state for all temperatures except T=0 is notably absent. The gas does not condense. This is due to a constant DOS even for E → 0, allowing a distribution of the particles to the excited states at any temperature T>0.
Hence, there exists *no BEC* in a homogenous 2D system for any finite temperature.

Again, investigating the phase of the order parameter, one can show that in an infinite 2D system a continuous symmetry can not be spontaneously broken. This means that for any distance r → ∞, the correlation function $g_1(r) ∝ exp(-r/l_c)$ vanishes exponentially for any correlation length $l_c(T≢0)$. This has been shown for the 2D Heisenberg model by Mermin and Wagner @Mermin1966, applied to 2D quantum field theory @Coleman1973 and rigorously proven for any 2D system by Hohenberg @Hohenberg1967. Thus, this gas does exhibit *no long range order*.

A qualitatively different behavior occurs if the particles of the 2D Bose gas are interacting with each other. Now, the correlation function $g_1(r)$ does not decay exponentially but only algebraically $g_1(r) ∝ (ξ/r)^α$. Since the correlations decays slowly this situation is called quasi long range order (QLRO).
Surprisingly, this gas is superfluid. In fact, the occurrence of a superfluid density $n_s$ is intimately linked to the existence of QLRO. If the correlations decay exponentially, the gas is in a thermal state. If the correlations decay algebraically, the gas is in the superfluid regime.

Interestingly, an unusual phase transition accompanies the change from exponential to algebraic decay of phase correlations. It is special in the sense that the change from a high temperature normal state to a low temperature superfluid state can not involve any spontaneous symmetry breaking. This transition is explained by the theory of Berezinskii @Berezinskii1971a, Kosterlitz and Thouless @Kosterlitz2002 This quantum phase transition revolves around another source of phase fluctuation, vortices. As will be shown later, the binding of vortices of opposite charge defines the transition from a normal fluid to a superfluid.

In the following, these points will be describes in more detail. Starting with the comparison of infinite homogeneous 3D and 2D gases and then introducing interactions. Concluding, the 2D case will be examined in the presence of a trapping potential and some finite size effects will be discussed.

## The Ideal 3D Gas

Interestingly the framework of classical statistical mechanics with the use of a grand canonical ensemble describes many important properties of a cold atom gas. From this, given the inverse temperature $β=(k_B T)^{-1}$ and the chemical potential $μ$ the average occupancy of a single particle state $ν$ with energy $ϵ$ can be derived as:

$$ f(ϵ_ν) = (ⅇ^{β(ϵ_ν-μ)}±γ)^{-1} \quad\quad μ=\left(\frac{∂E}{∂N}\right)_{S,V} $$ {#eq:meanoccupation}

Here, the chemical potential has to be evaluated at constant entropy $S$ and volume $V$. The constant $γ$ describes the nature of the distribution the particles

\begin{align}
γ =& +1       : \text{Fermi-Dirac}\\
γ =&\quad\, 0 : \text{Maxwell-Boltzmann}\\
γ =& -1       : \text{Bose-Einstein}
\end{align}

Note, since $ϵ ≥ 0$ when the single particle spectrum starts at $ϵ_0 = 0$ and the occupation is per defintion positive one immediately requires $-∞ ≤μ ≤ 0$ for the Bose-Einstein distribution. For the other distributions, the chemical potential can take on either sign. In @Fig:meanoccupancy the different behaviours of the distributions for small $β(ϵ_ν-μ)$ are shown.

![Mean Occupancy](/Volumes/Data/Jonas/Documents/latex/phd_thesis_markdown/images/2016/07/MeanOccupancy.png){#fig:meanoccupancy}

From this, basic properties of the gas can be calculated. Like the mean energy $E$

$$ E = ∑_ν ϵ_ν f(ϵ_ν),$$ {#eq:meanenergy}

or the mean particle number

$$ N = ∑_ν f(ϵ_ν).$$ {#eq:meanparticlenumber}

If the temperature of the system is sufficiently high or the size is sufficiently large, the spacing of the single-particle energy levels becomes small enough to replace the sum over discrete states by an integral over the energy weighted by the density of states $g(ϵ)$. Hence, the particle number - for example -- can be written like

$$ N = ∑_ν f(ϵ_ν) ≈ ∫_0^∞ f(ϵ) g(ϵ) \text{d}ϵ $$



Table \ref{ref_a_table} shows us how to add a table.

<!-- \newpage -->

-----------------------------------------------------------
                      Ideal 3D Gas            Ideal 2D Gas                
----------------      --------------      ------------------    
Condensation          Yes                 No

Long Range Order      Yes                 No    

Superfluidity         No                  No          

--------------   -------------------------------------------

Table: Comparison of Coherence and superfluidity in ideal 3D/2D gases. \label{ref_a_table}

-----------------------------------------------------------
                      Interacting 3D Gas  Interacting 2D Gas                
----------------      --------------      ------------------    
Condensation          Yes                 No

Long Range Order      Yes                 Quasi   

Superfluidity         Yes                 Yes         

--------------   -------------------------------------------

Table: Comparison of Coherence and superfluidity in interacting  3D/2D gases. \label{ref_a_table}
