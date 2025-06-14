# Square Quantum Well Energy Levels

## Objective
Determine all energy levels of an electron in a Square Quantum Well (SQW) for various well widths and visualize the relationship between energy levels and well width dimensions.

## Problem Description
Using the program developed in the lab session as a foundation, calculate and analyze the energy spectrum of electrons confined in square quantum wells with widths ranging from 5 nm to 100 nm.

## Requirements

### Simulation Parameters
- **Well Width Range**: 5 nm to 100 nm
- **Width Increment**: 5 nm steps
- **Energy Discretization**: Refined as necessary for accurate results
- **Output Format**: A4 sheet presentation with comprehensive analysis

### Computational Tasks
1. **Energy Level Calculation**
   - Solve Schrödinger equation for each well width
   - Determine all bound energy states
   - Ensure numerical accuracy through appropriate discretization

2. **Data Collection**
   - Calculate energy levels for 20 different well widths (5, 10, 15, ..., 100 nm)
   - Store results for each quantum state (n = 1, 2, 3, 4, ...)
   - Handle cases where higher states don't exist for narrow wells

3. **Visualization Requirements**
   - **X-axis**: Well width (nm)
   - **Y-axis**: Energy levels (eV)
   - **Multiple curves**: Each energy level (1st, 2nd, 3rd, etc.) as separate colored lines
   - **Curve behavior**: Monotonically decreasing functions
   - **Curve hierarchy**: Higher energy levels start at larger well widths

## Implementation Steps

### 1. Program Modification
- Build upon the lab session's Schrödinger equation solver
- Implement well width parameterization
- Add energy level extraction functionality

### 2. Numerical Considerations
- **Energy discretization**: Refine grid spacing for accurate eigenvalue determination
- **Convergence criteria**: Ensure numerical stability across different well widths
- **Boundary conditions**: Proper implementation of infinite potential walls

### 3. Data Processing
- **State identification**: Correctly label quantum states (n = 1, 2, 3, ...)
- **Missing states**: Handle cases where higher states don't exist for narrow wells
- **Data validation**: Verify physical consistency of results

### 4. Graph Construction
- **Multi-curve plotting**: Different colors for each energy level
- **Professional formatting**: Suitable for A4 presentation
- **Clear labeling**: Axes, legend, and curve identification

## Expected Physical Behavior

### Energy-Width Relationship
The energy levels follow the relationship:
```
E_n = (n²π²ℏ²)/(2mL²)
```
Where:
- `n` = quantum number (1, 2, 3, ...)
- `ℏ` = reduced Planck constant
- `m` = electron mass
- `L` = well width

### Key Observations
1. **Inverse Relationship**: Energy levels decrease as well width increases (∝ 1/L²)
2. **State Emergence**: Higher energy levels appear only for sufficiently wide wells
3. **Level Spacing**: Energy spacing decreases with increasing well width
4. **Monotonic Behavior**: All curves are monotonically decreasing

## Graph Characteristics

### Visual Features
- **Curve Colors**: Distinct colors for each energy level (n = 1, 2, 3, ...)
- **Curve Order**: Higher energy curves positioned above lower ones
- **Starting Points**: Higher energy levels begin at larger well widths
- **Convergence**: All curves show decreasing energy with increasing width

### Professional Presentation
- **Format**: Suitable for A4 sheet
- **Clarity**: Clear legends and axis labels
- **Completeness**: All calculated energy levels are represented

## Commentary Analysis

### Physical Insights
1. **Quantum Confinement**: Demonstrates how spatial confinement quantizes energy
2. **Size Effects**: Shows the relationship between nanostructure dimensions and electronic properties
3. **State Density**: Illustrates how energy level density increases with well width
4. **Threshold Behavior**: Higher states require minimum well widths to exist

### Practical Applications
- **Quantum Dot Design**: Understanding size-dependent electronic properties
- **Semiconductor Engineering**: Tailoring energy levels through dimensional control
- **Device Optimization**: Predicting electronic behavior in confined structures

## Success Criteria

### Computational Accuracy
- Correct implementation of the Schrödinger equation solver
- Appropriate numerical discretization
- Physically consistent results

### Visualization Quality
- Professional graph suitable for A4 presentation
- Clear representation of all energy levels
- Proper curve ordering and coloring

### Analysis Depth
- Comprehensive commentary on physical behavior
- Explanation of observed trends
- Connection to quantum mechanical principles

## Technical Specifications

### Units and Constants
- **Length**: nanometers (nm)
- **Energy**: electron volts (eV)
- **Mass**: Electron rest mass (9.109 × 10⁻³¹ kg)
- **Planck constant**: ℏ = 1.055 × 10⁻³⁴ J·s

### Numerical Parameters
- **Grid spacing**: Sufficient for convergence
- **Energy resolution**: Adequate for level identification
- **Well depth**: Infinite (hard walls)
