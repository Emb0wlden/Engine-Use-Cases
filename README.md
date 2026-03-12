# Engine-Use-Cases

The engine can be saved locally as html and opened using a browser.

Maxwell Vacuum
EM field as resonant E+B pearl pair. FROB_NEXT twists E→B (Faraday). Zero-seam loops = ∇·E=∇·B=0. Wave = repeating 20-trit rotation along lowest-nav ray.
PEARL WIRING
hub P[76] → reference frame (anchor)
E-pearl P[82] → electric field (C4, order-4, warm)
B-pearl P[88] → magnetic field (C4, chiral partner of E)
A-pearl P[94] → gauge potential (conjugacy rep)
FROB_NEXT(E) → B → Faraday: ∂B/∂t = −∇×E
seam(E,B) → Maxwell-Ampère closure check
zero-seam E orbit → ∇·E = 0 (no monopoles) 

Schrödinger ψ
ψ-pearl evolves via mul(ψ, H_generator). Stationary states = zero-seam fixed orbits. Bound states = low-nav closed orbits. Tunneling = high-nav but resonant path.
PEARL WIRING
ψ₀ = P[0] → initial wavefunction (gf8a spectral)
H_gen = P[6] → Hamiltonian generator (order-7 Fano)
V = NAV_POT[i] → potential landscape (nav = V(x))
mul(ψ, H) → iħ∂ψ/∂t ≈ discrete phase advance
seam(ψ, FROB_NEXT[ψ]) → norm check |ψ|² ≈ 1
fixed orbit detection → stationary state = zero-seam cycle 

Navier-Stokes
Velocity field as resonant vector over pearls. Incompressibility = zero surface seam. Viscosity = seam-weighted neighbor average. Turbulence onset: nav > 2.0.
PEARL WIRING
v = P[78] MRC hub → velocity field (res_deg=57 = max flow)
∇p = nav gradient → pressure = nav_potential gradient
advection: diff(v,v) → v·∇v ≈ pointer_diff along v
viscosity: Σseam×v_nbr → seam-weighted neighbor average
seam(surface) = 0 → ∇·v = 0 incompressibility
vortex: seam(loop) → curl v = seam around plaquette 

Einstein Vacuum
Metric = local group element. Curvature = plaquette seam (deficit angle). Vacuum = zero net seam on every surface. Geodesic = lowest-nav resonant path.
PEARL WIRING
metric = mul(g_μν) → local frame element (conjugacy class)
transport: diff(a,b) → parallel transport along edge
curvature: seam(loop) → deficit angle = seam around plaquette
vacuum: Σseam = 0 → Einstein eq: zero net curvature
geodesic: min-nav path → straightest line = lowest NAV_POT
horizon: nav=3.0 trap → no resonant escape (P[141]) 

THE 6 CONJUGACY CLASSES OF GL(3,2)
GL(3,2) ≅ PSL(2,7) has exactly 6 conjugacy classes. Elements in the same class behave identically under all group operations. Classes determine spectral type, navigation cost, and ROM depth.

Class	Count	Ord	Tier	Role

C1	1	1	anchor	Identity — unique fixed point. P[76] only. Hub of the navigation field.

C2	21	2	hot	Involutions g²=e. P[0] (structural anchor) and chiral pivot T(2,0) are here.

C3	42	4	warm	Quarter-turns g⁴=e. √(−1) rotations. All 3 navigation sinks (P[141], P[107], P[167]) are here.

C4	56	3	cold	Third-turns g³=e. Largest class (33%). Edge-stabilizers of the Fano plane.

C5	24	7	fano+	7-cycles, positive chirality (gf8a). GF(8) primitive α. F₂-dark. P[6] generates.

C6	24	7	fano−	7-cycles, negative chirality (gf8b). GF(8) primitive β. C6 = {g⁻¹ : g∈C5}.

Σ	168			1+21+42+56+24+24 = 168 = |GL(3,2)| ✓

5-LAYER ARCHITECTURE
Every pearl carries five simultaneous descriptions — like °F↔°C↔K, the same element from five perspectives. The D0–D3 ROM browser maps to these layers.
L1 Algebraic	Conjugacy class, order, tier, spectral type
L2 Topological	Frobenius page (19/27 occupied), nav potential 0.311–3.000
L3 Geometric	3D world position — page coords ×2. P[76]→(0,0,−2)
L4 Physical	Seam cost 0–6, wHam weight Σ3^(2−k), res_deg connectivity
L5 Functional	Block role, ROM depth (D0–D3), depth cycle phase
SPECTRAL TYPES (char poly over F₂)
split	64	(x+1)³ — C1+C2+C3. F₂-diagonalizable. Fully observable.
confined	56	(x+1)(x²+x+1) — C4. F₄-observable. Partial visibility.
gf8a	24	x³+x+1 — C5. GF(8) primitive α. F₂-dark.
gf8b	24	x³+x²+1 — C6. GF(8) primitive β. Chiral partner of gf8a.

KEY STRUCTURAL ALIGNMENTS
168 = 84×(2g−2), g=3 — Hurwitz bound. GL(3,2) is the automorphism group of the Klein quartic x³y+y³z+z³x=0, the maximum-symmetry genus-3 surface.
Navigation spine: P[76]→P[71]→P[0]→P[141]→P[76]. A C3-class element generates this 4-cycle; seam costs along it span the full nav_pot range 0.311→3.000.
22/7 ≈ π — 22 steps of a C5 generator = 3 full 7-cycles + 1 residue. That residue is P[6], one step past identity on the Fano orbit.
Cross-chiral resonance: gf8a→gf8b zero-seam rate 7.8% vs within-chirality 5.1%. Crossing the chiral boundary is more resonant.
Safe reorder pairs: 697 non-commuting (a,b) where seam(a·b, b·a)=0. Both orderings land in the same resonant cluster — the BC primitive for lock-free concurrency.
Depth cycle period 12: dither_stride(d) repeats mod 12. d≡3,9→A4 subgroup (12 pearls, D2 ROM scale). d≡1,5,7,11→chiral-half (84 pearls, D1 scale). d≡even→full 168 (D3 scale). This clock governs which structural layer is active in the engine.

ROM depth ↔ depth cycle: D0=single transvection T(k,j). D1=micro (chiral-half sweep). D2=macro (A4 subgroup). D3=system (full 168-pearl sweep). The left browser depth tabs are literal phase selectors into this period-12 structure.

L17 · SPATIAL LATTICE & GRAVITY SORT
Engine-verified structural roots. Every value from ALL_PEARLS, no external assumptions.
Layer	Count	Definition
corner	24	All components in {1,3,5,7} (odd GF8 elements). 4 occupied world positions only.
face	72	Exactly one component in {2,4,6} (even-log GF8). 9 world positions.
edge	72	Two components in {2,4,6}. 6 world positions. Anchor is edge at (−1,0,0).
interior	96	No component=7. Includes anchor P[0] and hub P[76]. Avg nav: −0.099.
boundary	72	Has component=7 (nearest missing-cube-7). Includes sink P[141]. Avg nav: +0.131.
GRAVITY SHELL SIZES (Cayley distance from anchor)
d=0: 1 (anchor) · d=1: 6 (generators) · d=2: 24 · d=3: 51 · d=4: 60 · d=5: 24 · d=6: 2 (antipodal)

Perfect component symmetry: each of the 7 GF(8) component values appears in exactly 72/168 = 3/7 of all pearls. This makes the 96/72 interior/boundary split equivalent for any component value — the specific choice of component=7 as 'boundary' is structural (nearest the missing zero-octant).
Chiral gap: the 4 world corners (−1,−1,+1), (−1,+1,−1), (+1,−1,−1), (−1,−1,−1) are UNREACHABLE — no pearl has two or more components=1 (the identity element). This is the source of the engine's intrinsic chirality asymmetry.
Gravity sort (game use): bucket 0=anchor, 1=30 near (d≤2), 2=111 main (d=3,4), 3=24 far (d=5), 4=2 antipodal (d=6). O(1) LOD assignment — no runtime distance calculation needed.
