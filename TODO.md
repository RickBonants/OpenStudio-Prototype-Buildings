## TODO

### Workflow

- Create a branch for each new feature
- Pull request to Master after feature is complete
- Pull request to Master ASAP after changing a spreadsheet
- When spreadsheet, color the cells for later conflict resolution purposes
	- NREL- Blue
	- ORNL - Green
	- LBL - Background yellow
- Make commit messages clear, favoring clarity over brevity

### Building Type Assignments

##### NREL
- Small Office
- Secondary School
- Primary School

##### ORNL
- Medium Office
- Large Office
- Warehouse (non-refrigerated)

##### LBL
- Small Hotel
- Large Hotel

##### Unassigned
- Stand-alone Retail
- Strip Mall
- Outpatient Healthcare
- Hospital
- Quick Service Restaurant
- Full Service Restaurant
- Mid-rise Apartment
- High-rise Apartment

#### General TODO
- [x] Generalize spreadsheet export
- [X] Flatten file structure to meet Measure requirements
- [ ] Chillers for Pre-1980 and 1980-2004
- [ ] DX Heating coil efficiency
- [ ] Check if two sizing runs necessary and remove one if not
- [ ] Merge schedules to standards spreadsheet, leave HVAC and prototype inputs
- [ ] Generalize standards spreadsheet JSON export to match hvac standards spreadsheet and add units to headers
- [ ] Make 90.1-2004-2010 space type templates use schedules pulled from prototype bldgs
- [ ] Scrape constructions and materials from prototype IDFs for 90.1-2004-2010
- [ ] Put standards R-values in for Constructions instead of building up layer-by-layer in spreadsheet?
- [ ] Run all legacy IDF files
- [ ] Make spreadsheet export use cross-platform Ruby gem
- [ ] Make sure that tests run in Ruby 2.0.0 (OS 1.5.+)

#### Building Specific TODO

##### SmallOffice

- [ ] DX Cooling Coil Efficiency Lookup for 90.1-2010
  - [ ] COP 3.91 in legacy vs. 3.0 in mine
- [ ] DX Heating Coil Efficiency Lookup for 90.1-2010
  - [ ] COP 3.29 in legacy vs. 5.0 in mine
- [x] ~~Zero out SWH pump head~~
- [x] ~~Set water heater efficiency to 1 and thermal efficiency to 0.99 if electric~~
- [ ] Figure out why design loads is higher in legacy
  - [ ] check envelope
  - [ ] fix envelope
    - [ ] Pre1980 uses steel frame walls, IEAD roof
    - [ ] 1980-2004 uses mass walls, attic roof
    - [ ] 90.1-200-90.1-2010 uses wood frame walls, attic roof
    - [ ] OpenStudio uses mass walls, attic roof
    - [ ] need to add attic construction set
- [ ] check infiltration
- [ ] check loads
- [ ] Add infiltration to Zn 1 for Door
