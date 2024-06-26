# Codebook – Created 04/02/2024
## Dataset: ACSPUMS1Y2022

### Variables:
- **VALP** - Property value
  - **Topics**: Financial Characteristics, Housing Value and Purchase Price
  - **Suggested Weight**: WGTP
  - **Description**: Property value
  - **Values**:
    - 0 - N/A (GQ/vacant units, except 'for-sale-only' and 'sold, not occupied'/not owned or being bought)
    - 1,9999999 - $1 to $9999999 (Rounded and top-coded)

- **SEX** - Sex
  - **Topics**: Age and Sex, Populations and People
  - **Suggested Weight**: PWGTP
  - **Description**: Sex Variable Universe Description: ALL
  - **Values**:
    - 1 - Male
    - 2 - Female

- **JWTRNS** - Means of transportation to work
  - **Topics**: Commuting
  - **Suggested Weight**: PWGTP
  - **Description**: Means of transportation to work
  - **Values**:
    - 0 - N/A (not a worker-not in the labor force, including persons under 16 years; unemployed; employed, with a job but not at work; Armed Forces, with a job but not at work)
    - 01 to 12 - Specific modes of transport (Car, Bus, etc.)

- **COW** - Class of worker
  - **Topics**: Class of Worker
  - **Suggested Weight**: PWGTP
  - **Description**: Class of worker
  - **Values**:
    - 0 to 9 - Specific classifications (Private company, Government, Self-employed, etc.)

- **AGEP** - Age
  - **Topics**: Age and Sex, Populations and People
  - **Suggested Weight**: PWGTP
  - **Description**: Age
  - **Values**:
    - 00 - Under 1 year
    - 1,99 - 1 to 99 years (Top-coded)

- **DIS** - Disability recode
  - **Topics**: Disability
  - **Suggested Weight**: PWGTP
  - **Description**: Disability recode
  - **Values**:
    - 1 - With a disability
    - 2 - Without a disability

- **MIL** - Military service
  - **Topics**: Veterans
  - **Suggested Weight**: PWGTP
  - **Description**: Military service
  - **Values**:
    - 0 to 4 - Specific classifications (Active duty, Reserves, etc.)

- **MARHT** - Number of times married
  - **Topics**: Marital Status and Marital History
  - **Suggested Weight**: PWGTP
  - **Description**: Number of times married
  - **Values**:
    - 0 to 3 - Specific counts (Never married, Once, Twice, etc.)

- **SCHL** - Educational attainment
  - **Topics**: Education, Educational Attainment
  - **Suggested Weight**: PWGTP
  - **Description**: Educational attainment
  - **Values**:
    - 0 to 24 - Specific levels (No schooling, Nursery, Kindergarten, up to Doctorate degree)

- **PWGTP** - PUMS person weight
  - **Topics**:
  - **Description**: PUMS person weight Variable Universe Description: ALL
  - **Valid Range**: 1 to 9,999
  - **Values**:
    - 1,9999 - Continuous values of PWGTP

- **WKHP** - Usual hours worked per week past 12 months
  - **Topics**: Employment, Usual Hours and Weeks Worked, Work Experience
  - **Suggested Weight**: PWGTP
  - **Description**: Usual hours worked per week past 12 months
  - **Values**:
    - 0 - N/A (less than 16 years old/did not work during the past 12 months)
    - 99 - 99 Or More Usual Hours
    - 1,98 - 1 to 98 usual hours

- **NATIVITY** - Nativity
  - **Topics**: Native and Foreign Born
  - **Suggested Weight**: PWGTP
  - **Description**: Nativity
  - **Values**:
    - 1 - Native
    - 2 - Foreign born

- **VEH** - Vehicles (1 ton or less) available
  - **Topics**: Physical Characteristics
  - **Suggested Weight**: WGTP
  - **Description**: Vehicles (1 ton or less) available
  - **Values**:
    - -1 - N/A (GQ/vacant)
    - 0 - No vehicles
    - 1 to 6 - 1 vehicle, 2 vehicles, up to 6 or more vehicles

- **WAGP** - Wages or salary income past 12 months (use ADJINC to adjust WAGP to constant dollars)
  - **Topics**: Income and Earnings
  - **Suggested Weight**: PWGTP
  - **Description**: Wages or salary income past 12 months
  - **Values**:
    - -1 - N/A (less than 15 years old)
    - 0 - None
    - 4 to 999999 - $4 to $999999 (Rounded and top-coded)

- **RNTP** - Monthly rent (use ADJHSG to adjust RNTP to constant dollars)
  - **Topics**: Financial Characteristics, Renter Costs
  - **Suggested Weight**: WGTP
  - **Description**: Monthly rent (use ADJHSG to adjust RNTP to constant dollars)
  - **Values**:
    - 0 - N/A (GQ/vacant units, except "for rent" and "rented, not occupied"/owned or being bought/occupied without rent payment)
    - 1 to 99999 - $1 to $99999 (Rounded and top-coded)

- **MAR** - Marital status
  - **Topics**: Marital Status and Marital History
  - **Suggested Weight**: PWGTP
  - **Description**: Marital status Variable Universe Description: ALL
  - **Values**:
    - 1 - Married
    - 2 - Widowed
    - 3 - Divorced
    - 4 - Separated
    - 5 - Never married or under 15 years old

- **ENG** - Ability to speak English
  - **Topics**: Language Spoken at Home, Native and Foreign Born
  - **Suggested Weight**: PWGTP
  - **Description**: Ability to speak English
  - **Values**:
    - 0 - N/A (less than 5 years old/speaks only English)
    - 1 - Very well
    - 2 - Well
    - 3 - Not well
    - 4 - Not at all

### Selected Geographies (ucgid):
- **795P200US4805302** -- Austin City (North) PUMA; Texas
- **795P200US4805307** -- Austin City (South) PUMA; Texas
- **795P200US4805306** -- Austin City (Central) PUMA; Texas
