# Shape Memory Alloy Dataset - Merge Summary Report

## Overview
Successfully combined **84 CSV files** from 4 source directories into a single comprehensive dataset.

## Output File
- **File**: `Combined_SMA_Dataset.csv`
- **Total Records**: 17,258
- **Total Columns**: 34
- **File Size**: 4.33 MB

## Source Directories Merged

| Directory | Description | Records | Files |
|-----------|-------------|---------|-------|
| AF_MF_ALL | Austenite Finish & Martensite Finish Temperatures | 4,201 | 23 |
| AS_MS_ALL | Austenite Start & Martensite Start Temperatures | 4,785 | 26 |
| CR_HR_ALL | Cooling Rate & Heating Rate | 4,340 | 19 |
| TSPAN_CD_ALL | Thermal Span & Calculated Density | 3,932 | 16 |

## Field Structure (34 Columns)

### 1. Metadata Fields (2)
- `Source_Directory` - Origin directory of the data
- `Alloy_Type` - Name of the alloy system

### 2. Universal Fields (5)
Present in all original CSV files:
- `Authors` - Research authors
- `Source` - Publication source
- `Title` - Paper title  
- `Year` - Publication year
- `composition` - Chemical composition description

### 3. Element Composition Fields (19)
Atomic percentage of elements:
- `Ag (at.%)`
- `Al (at.%)`
- `Au (at.%)`
- `Cd (at.%)`
- `Co (at.%)`
- `Cu (at.%)`
- `Fe (at.%)`
- `Hf (at.%)`
- `Mn (at.%)`
- `Nb (at.%)`
- `Ni (at.%)`
- `Pd (at.%)`
- `Pt (at.%)`
- `Ru (at.%)`
- `Si (at.%)`
- `Ta (at.%)`
- `Ti (at.%)`
- `Zn (at.%)`
- `Zr (at.%)`

### 4. Temperature Measurement Fields (4)
Phase transformation temperatures:
- `Austenite Finish Temperature - AF - (°C)`
- `Austenite Start Temperature - AS - (°C)`
- `Martensite Finish Temperature - MF - (°C)`
- `Martensite Start Temperature - MS - (°C)`

### 5. Rate Fields (2)
Thermal processing rates:
- `Cooling Rate (°C/min)`
- `Heating Rate (°C/min)`

### 6. Other Measurement Fields (2)
- `Calculated Density (g/cm^3)`
- `Thermal transformation span (TSPAN) - (AF-MF) - (°C)`

## Data Characteristics

### Unique Compositions
- Total unique compositions: 1063

### Top 10 Alloy Systems by Record Count
1. **NiTiHf**: 4,461 records
2. **NiTiCu**: 3,468 records
3. **NiTiPd**: 1,519 records
4. **NITiCu**: 1,224 records
5. **NiTiZr**: 1,153 records
6. **NiTi**: 834 records
7. **NiTiNb**: 811 records
8. **NiTiAu**: 757 records
9. **FeMnSi**: 471 records
10. **CuAlMn**: 356 records

### Records by Source Directory

- **AF_MF_ALL**: 4,201 records (24.3%)
- **AS_MS_ALL**: 4,785 records (27.7%)
- **CR_HR_ALL**: 4,340 records (25.1%)
- **TSPAN_CD_ALL**: 3,932 records (22.8%)

## Field Coverage Analysis

### Fields Present in All Records (Universal)
- Source_Directory
- Alloy_Type
- Authors
- Source
- Title
- Year
- composition

### Directory-Specific Fields
Different measurements are available depending on source directory:

**AF_MF_ALL records contain:**
- Austenite Finish Temperature - AF - (°C)
- Martensite Finish Temperature - MF - (°C)

**AS_MS_ALL records contain:**
- Austenite Start Temperature - AS - (°C)
- Martensite Start Temperature - MS - (°C)

**CR_HR_ALL records contain:**
- Cooling Rate (°C/min)
- Heating Rate (°C/min)

**TSPAN_CD_ALL records contain:**
- Thermal transformation span (TSPAN) - (AF-MF) - (°C)
- Calculated Density (g/cm^3)

### Element Composition Coverage
Element fields are populated only for alloys containing those elements.

## Data Quality Notes

1. **No Data Loss**: All 17,258 records from all 84 source files are preserved
2. **Field Preservation**: All 34 unique fields across all files are included
3. **Empty Cells**: Records contain empty values for fields not applicable to their source directory or alloy composition
4. **Multiple Measurements**: Same compositions may appear multiple times from different research papers/years
5. **Source Tracking**: `Source_Directory` and `Alloy_Type` fields allow tracing back to original files

## Usage Recommendations

1. **Filtering**: Use `Source_Directory` to filter for specific measurement types
2. **Alloy Analysis**: Use `Alloy_Type` to focus on specific alloy systems  
3. **Research Tracking**: Use `Authors`, `Source`, `Title`, `Year` for citation and source verification
4. **Composition Analysis**: Element fields enable compositional studies
5. **Missing Data**: Check for empty values when performing analysis on directory-specific fields

## File Location
```
/home/user/Shape-Memory-Alloy-Dataset/Combined_SMA_Dataset.csv
```

---
*Generated on: 2025-11-15*
*Merge operation completed successfully*
