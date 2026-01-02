```mermaid
graph TD

    %% 1. Input Layer
    subgraph Inputs ["External Inputs"]
        A1[Solar Energy] --> B1
        A2[Rainwater Collection] --> B2
        A3[Barley Seeds] --> B3
    end

    %% 2. Energy & Thermal Management
    subgraph Energy ["Energy & Thermal Loop"]
        B1[150kW Solar Array] --> B4[Battery Storage - 250kWh]
        B4 --> B5[Facility Power Grid]
        B6[Thermal Heat Exchanger] -- "Waste Heat" --> C1
        B5 --> D3[3D Printer Array]
        B5 --> D1[Industrial Mill]
    end

    %% 3. Biological Engine
    subgraph Biology ["Closed-Loop Biological Engine"]
        C1[Beetle Nursery - 82°F] -- "Eggs" --> C2[Larvae Growth Chamber]
        C2 -- "1% Diversion" --> C3[Pupation Chamber]
        C3 -- "Adults" --> C1
        
        B3[Barley Seeds] --> B2[Hydroponic Fodder Racks]
        B2 -- "Biomass" --> C2
        
        C2 -- "Frass - Fecal Matter" --> C4[Vibrating Sieve]
        C4 -- "Liquid NPK" --> B2
    end

    %% 4. Fabrication & Processing
    subgraph Fabrication ["Food Fabrication & Stabilizers"]
        C2 -- "Harvested Larvae" --> D1[Steam Blancher / Mill]
        D1 -- "Protein Flour" --> D3
        
        E1[Algae Photobioreactor] -- "Agar" --> D3
        E2[Guar Hydroponics] -- "Guar Gum" --> D3
        
        D3[Industrial 3D Printers] -- "Texture/Nutrients" --> F1[Nutri-Brick Meals]
    end

    %% 5. Distribution & Economic Loop
    subgraph Economics ["Economic & Distribution Loop"]
        F1 --> G1[Packaging Media Unit]
        G1 -- "Ad-Stamping" --> G2[Revenue: $0.15/meal]
        G1 -- "Final Product" --> H1[SC Prison System]
        G1 --> H2[Homeless Networks / I-95 Corridors]
        
        C4 -- "Bulk Fertilizer" --> G3[Local SC Farm Sales]
        B1 -- "Net Metering" --> G4[Carbon Credits]
    end

    %% Systemic Connections
    D3 -- "Friction Heat" --> B6
    D1 -- "Friction Heat" --> B6
    C1 -- "CO2" --> B2

    C2 -- "CO2" --> E1

