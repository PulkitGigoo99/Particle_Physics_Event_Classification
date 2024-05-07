# Particle Physics Event Classification

## Problem Statement:

1. In the field of particle physics, accurate identification and classification of events are crucial for understanding fundamental particles and their interactions. 
2. The provided dataset contains various features derived from particle physics experiments
3. The goal is to build a machine-learning model to classify events into signal (s) and background (b) categories. This classification aids in distinguishing events of interest (signal) from background noise.

## Data Description:

    EventId: Identifier for each event in the experiment.
    
    DER_mass_MMC: Derived mass of the Missing Mass Calculator. Represents the calculated mass of a system using the missing energy in the experiment.
    
    DER_mass_transverse_met_lep: Indicates the mass calculated from the transverse components of missing energy and lepton.
    
    DER_mass_vis: Derived mass of the visible part of the system. Represents the mass of the visible particles in the system, excluding invisible or undetected 
    particles.
    
    DER_pt_h: Transverse momentum of the Higgs boson. Indicates the momentum of the Higgs boson in the transverse plane, providing information about its motion.
    
    DER_deltaeta_jet_jet: The absolute difference in pseudorapidity between the two jets.Describes the angular separation between two jets in the experiment.
    
    DER_mass_jet_jet: Derived mass of the two jets.

    DER_lep_eta_centrality: Pseudorapidity centrality of the lepton concerning jets.Pseudorapidity is a spatial coordinate used in particle physics. This feature 
    likely indicates the centrality of the lepton (a charged particle, possibly an electron or a muon) concerning jets in the event. The centrality provides 
    information about the lepton's position relative to the jets.
    
    PRI_tau_pt: Transverse momentum of the tau.Transverse momentum is the momentum of a particle in the direction perpendicular to the beamline. This feature 
    represents the transverse momentum of the tau particle, which is a heavy, charged particle often involved in processes like tau decays.
    
    PRI_tau_eta: Pseudorapidity of the tau.Pseudorapidity is a measure of the angle of a particle's trajectory relative to the beamline. This feature indicates the 
    pseudorapidity of the tau particle, providing information about its direction.
    
    PRI_tau_phi: Azimuthal angle of the tau.Azimuthal angle defines the rotation of a particle's trajectory around the beamline. This feature represents the 
    azimuthal angle of the tau particle, indicating its orientation in the transverse plane.

    PRI_lep_pt: Transverse momentum of the lepton.Similar to PRI_tau_pt, this feature represents the transverse momentum of the lepton (electron or muon) in the 
    event.

    PRI_lep_eta: Pseudorapidity of the lepton.Similar to PRI_tau_eta, this feature indicates the pseudorapidity of the lepton, providing information about its 
    angular position relative to the beamline.

    PRI_lep_phi: Azimuthal angle of the lepton.Similar to PRI_tau_phi, this feature represents the azimuthal angle of the lepton, indicating its orientation in the 
    transverse plane.

    PRI_met: Missing transverse energy.Missing transverse energy is a crucial concept in particle physics. It represents the imbalance in transverse energy in an 
    event, suggesting the presence of undetected particles or neutrinos.
    
    PRI_met_phi: Azimuthal angle of the missing transverse energy.Similar to PRI_tau_phi and PRI_lep_phi, this feature represents the azimuthal angle of the 
    missing transverse energy, indicating its orientation in the transverse plane.
    
    PRI_met_sumet: Sum of the transverse energy of all objects in the event.This feature represents the sum of the transverse energy (energy component 
    perpendicular to the beamline) of all objects (particles) detected in the event. It provides a measure of the overall energy flow in the transverse plane.
    
    PRI_jet_num: Number of jets in the event.Indicates the count of jets observed in the event. Jets are collimated sprays of particles resulting from high-energy 
    interactions. Knowing the number of jets is crucial for understanding the event's characteristics.
    
    PRI_jet_leading_pt: Transverse momentum of the leading jet.Represents the transverse momentum of the jet with the highest transverse momentum in the event. The 
    leading jet is the one with the most significant momentum contribution.

    PRI_jet_leading_eta: Pseudorapidity of the leading jet.Indicates the pseudorapidity (angular position) of the leading jet, providing information about its 
    direction in the detector.
    
    PRI_jet_leading_phi: Azimuthal angle of the leading jet.Represents the azimuthal angle of the leading jet, indicating its orientation in the transverse plane.

    PRI_jet_subleading_pt: Transverse momentum of the subleading jet.Represents the transverse momentum of the second-highest transverse momentum jet in the event 
    (subleading jet).
    
    PRI_jet_subleading_eta: Pseudorapidity of the subleading jet.Indicates the pseudorapidity of the subleading jet, providing information about its angular 
    position in the detector.

    PRI_jet_subleading_phi: Azimuthal angle of the subleading jet.Represents the azimuthal angle of the subleading jet, indicating its orientation in the 
    transverse plane.
    
    PRI_jet_all_pt: Sum of the transverse momentum of all jets in the event.This feature represents the sum of the transverse momentum of all jets detected in the 
    event. It provides a measure of the overall transverse momentum contributed by all jets.

    Weight: A weight associated with each event.The weight is a numerical value assigned to each event. It is often used as a scaling factor to account for the 
    significance or importance of each event in the analysis. The weight may be applied during training and evaluation to adjust the contribution of each event to 
    the model.

    Target column(Label): The target variable, indicating the class or label of each event (s or b). This is the target variable where each event is labeled as 
    either signal (s) or background (b).

## Dataset Structure:

No of Columns- 33

No of records/rows- 250001


## Models Used:

1. Logistic Regression

2. Random Forest



