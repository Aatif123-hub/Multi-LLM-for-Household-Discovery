# Summary

### Summary of Entity Resolution

#### Direct Matching

**Objective:** Link records that directly match by name.

| Record ID | Full Name                  | Address                         | City                | State | ZIP    | SSN          | Other Info | Explanation                                                                 |
|-----------|----------------------------|---------------------------------|---------------------|-------|--------|--------------|------------|-----------------------------------------------------------------------------|
| A910195   | m g habte                  | 5800 Owensmouth Ave Apt 18      | WOODLAND HILLS      | CA    | 91367  | NaN          | NaN        | Same name with minor spelling differences and identical address.            |
| A924822   | mathew g habte             | 5800 owensmoth avn apt 18      | woodland hilhls     | calif.| 91367  | NaN          | NaN        |                                                                             |
| A976579   | northington h clarke       | 10128 capistrano ave            | SOUTH GATE          | CA    | 90280  | 26189770     | NaN        | Same name with minor spelling differences and identical SSN.               |
| A986974   | N H CLARKE                 | 21490 PIONEER RD                | Los Banos           | CA    | 93635  | 026-18-9770  | 19350613   |                                                                             |
| A959515   | Northington H Clare        | 21490 pioneer rd                | los banos           | cali  | 93635  | 26189770     | NaN        |                                                                             |
| A997180   | NORTHINGTON H CLARKE       | 3917 Del Rey Drv                | SAN BERNARDINO      | CA    | 92404  | 206-18-9770  | NaN        |                                                                             |
| B902944   | CASEY A GACKENBACH         | 2759 ascot dr                   | Cardiff By The Sea  | CA    | 92009  | (760)214.3372| NaN        | Same name with minor spelling differences and identical phone number.    |
| B930743   | CASEY A Gackenbach         | 45236 APTDO                     | SAN DIEGO           | C     | 92145  | 619-380-4576 | NaN        |                                                                             |
| B921886   | Shelley S RICHARDS         | 3307 SPINDLETOP CTQ             | manvel              | texags| 77578  | 281.623-0402 | NaN        | Same name with minor spelling differences and identical address.          |
| B943484   | shelley S richards          | 1818 BOX                        | LEANDER             | TEXAS | 7F8646 | (512)452.2110| NaN        |                                                                             |
| B990320   | Shelley S richards          | 3307 Spindletop Ct              | manvel              | tx    | 77578  | (281)623.0402| NaN        |                                                                             |
| B997328   | shelley S rihcards         | 3307 Spindletop Court           | MANVEL              | TX    | 77578  | 281.623.0402 | NaN        |                                                                             |
| B988617   | SHELLEY S Richards          | 8963 westbrok ct                | rancho cucamonga    | calif.| 91730  | 909-146.6573 | NaN        |                                                                             |
| A970015   | Shelley S Richards          | 3307 SPINDLTOP CT               | manvel              | texas | 77578  | 25996464     | 1950       |                                                                             |
| A981133   | SHELLEY S RICHARDS          | 3307 SPINDLETOP CT              | MANVEL              | TX    | 77578  | 29596446     | 18396      |                                                                             |

#### Indirect Matching

**Objective:** Perform indirect matching of records connected through an intermediary.

| Record ID | Full Name                  | Address                         | City                | State | ZIP    | SSN          | Other Info | Explanation                                                                 |
|-----------|----------------------------|---------------------------------|---------------------|-------|--------|--------------|------------|-----------------------------------------------------------------------------|
| A920309   | MATTIE M RAMIREZ           | 508 HOLLYWOOD ST                | TULELAKE            | CA    | 96134  | 23665462     | NaN        | Same SSN with minor spelling differences and identical address.           |
| A922114   | martha m otrres            | 4410 BROWNING DRV               | oxnard              | ca    | 93033  | 023-66-5462  | 19170401   |                                                                             |

#### Identify Households

**Objective:** Find records that form a household.

| Record ID | Full Name                  | Address                         | City                | State | ZIP    | SSN          | Other Info | Explanation                                                                 |
|-----------|----------------------------|---------------------------------|---------------------|-------|--------|--------------|------------|-----------------------------------------------------------------------------|
| B921886   | Shelley S RICHARDS         | 3307 SPINDLETOP CTQ             | manvel              | texags| 77578  | 281.623-0402 | NaN        | Different names but identical address indicating a household.              |
| B990320   | Shelley S richards          | 3307 Spindletop Ct              | manvel              | tx    | 77578  | (281)623.0402| NaN        |                                                                             |
| B997328   | shelley S rihcards         | 3307 Spindletop Court           | MANVEL              | TX    | 77578  | 281.623.0402 | NaN        |                                                                             |
| A970015   | Shelley S Richards          | 3307 SPINDLTOP CT               | manvel              | texas | 77578  | 25996464     | 1950       |                                                                             |
| A981133   | SHELLEY S RICHARDS          | 3307 SPINDLETOP CT              | MANVEL              | TX    | 77578  | 29596446     | 18396      |                                                                             |

#### Identify Household Moves

**Objective:** Find instances where a household has moved to a new address.

| Record ID | Full Name                  | Address                         | City                | State | ZIP    | SSN          | Other Info | Explanation                                                                 |
|-----------|----------------------------|---------------------------------|---------------------|-------|--------|--------------|------------|-----------------------------------------------------------------------------|
| A976579   | northington h clarke       | 10128 capistrano ave            | SOUTH GATE          | CA    | 90280  | 26189770     | NaN        | Same name with minor spelling differences and different addresses.         |
| A986974   | N H CLARKE                 | 21490 PIONEER RD                | Los Banos           | CA    | 93635  | 026-18-9770  | 19350613   |                                                                             |
| A959515   | Northington H Clare        | 21490 pioneer rd                | los banos           | cali  | 93635  | 26189770     | NaN        |                                                                             |
| A997180   | NORTHINGTON H CLARKE       | 3917 Del Rey Drv                | SAN BERNARDINO      | CA    | 92404  | 206-18-9770  | NaN        |                                                                             |

### Explanation

- **Direct Matching:** Records were matched based on similar names and identical addresses or SSNs.
- **Indirect Matching:** Records were matched through intermediary attributes such as SSN and address.
- **Identify Households:** Records were identified as forming a household based on different names but identical addresses.
- **Identify Household Moves:** Records were identified as indicating a household move based on the same names but different addresses.

This summary provides a comprehensive analysis of the records, accounting for inconsistencies, missing data, and spelling errors.

#
