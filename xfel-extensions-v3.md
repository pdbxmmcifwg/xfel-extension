# Category Group xfel_group


              Categories that describe X-ray Free Electron Laser (XFEL) data collection and experimental details.

---

## Category pdbx_serial_crystallography_data_reduction


               Data items in the PDBX_SERIAL_CRYSTALLOGRAPHY_DATA_REDUCTION category record
               details about data processing that are unique to XFEL experiments.
               These will compliment data recorded in category pdbx_diffrn_merge_stat.

---


```
     
         Example 1
     
         _pdbx_serial_crystallography_data_reduction.diffrn_id           1
         _pdbx_serial_crystallography_data_reduction.frames_total        7324430
         _pdbx_serial_crystallography_data_reduction.crystal_hits         1797503
         _pdbx_serial_crystallography_data_reduction.frames_indexed      578620
```


---

| Attribute | Key | Required | Type | Units | Enumerated | Bounded |
| --------- | --- | -------- | ---- | ----- | ---------- | ------- |
| crystal_hits | no | no | int | None | no | yes |
| diffrn_id | yes | yes | code | None | no | no |
| droplet_hits | no | no | int | None | no | yes |
| frames_failed_index | no | no | int | None | no | yes |
| frames_indexed | no | no | int | None | no | yes |
| frames_total | no | no | int | None | no | yes |
| frame_hits | no | no | int | None | no | yes |
| lattices_indexed | no | no | int | None | no | yes |
| xfel_pulse_events | no | no | int | None | no | yes |
| xfel_run_numbers | no | no | text | None | no | no |

---

#### _pdbx_serial_crystallography_data_reduction.crystal_hits


            For experiments in which samples are provided in a
            continuous stream, the total number of frames collected
            in which the crystal was hit.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_data_reduction.diffrn_id (key)


               The data item is a pointer to _diffrn.id in the DIFFRN
               category.



#### _pdbx_serial_crystallography_data_reduction.droplet_hits


            For experiments in which samples are provided in a
            continuous stream, the total number of frames collected
            in which a droplet was hit.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_data_reduction.frames_failed_index


            For experiments in which samples are provided in a
            continuous stream, the total number of data frames collected
            that contained a "hit" but failed to index.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_data_reduction.frames_indexed


            For experiments in which samples are provided in a
            continuous stream, the total number of data frames collected
            that were indexed.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_data_reduction.frames_total


            The total number of data frames collected for this
            data set.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_data_reduction.frame_hits


            For experiments in which samples are provided in a
            continuous stream, the total number of data frames collected
            in which the sample was hit.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_data_reduction.lattices_indexed


            For experiments in which samples are provided in a
            continuous stream, the total number of lattices indexed.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_data_reduction.xfel_pulse_events


            For FEL experiments, the number of pulse events in the dataset.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_data_reduction.xfel_run_numbers


               For FEL experiments, in which data collection was performed
	       in batches, indicates which subset of the data collected
               were used in producing this dataset.



## Category pdbx_serial_crystallography_measurement


               Data items in the PDBX_SERIAL_CRYSTALLOGRAPHY_MEASUREMENT category record
               details the beam that is impinging on the sample

---


```
     
         Example 1
     
         _pdbx_serial_crystallography_measurement.diffrn_id                1
         _pdbx_serial_crystallography_measurement.pulse_duration           45
         _pdbx_serial_crystallography_measurement.photons_per_pulse        0.17
         _pdbx_serial_crystallography_measurement.focal_spot_size          1.8
         _pdbx_serial_crystallography_measurement.collection_time_total   16.95
```


---

| Attribute | Key | Required | Type | Units | Enumerated | Bounded |
| --------- | --- | -------- | ---- | ----- | ---------- | ------- |
| collection_time_total | no | no | float | hours | no | yes |
| collimation | no | no | text | None | no | no |
| diffrn_id | yes | yes | code | None | no | no |
| focal_spot_size | no | no | float | micrometres_squared | no | yes |
| photons_per_pulse | no | no | float | teraphotons_per_pulse | no | yes |
| pulse_duration | no | no | float | femtoseconds | no | yes |
| pulse_energy | no | no | float | microjoules | no | yes |
| pulse_photon_energy | no | no | float | kiloelectron_volts | no | yes |
| source_distance | no | no | float | metres | no | yes |
| source_size | no | no | float | micrometres_squared | no | yes |
| xfel_pulse_repetition_rate | no | no | float | hertz | no | yes |

---

#### _pdbx_serial_crystallography_measurement.collection_time_total


            The total number of hours required to measure this data set.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_measurement.collimation


               The collimation or type of focusing optics applied to the radiation.



#### _pdbx_serial_crystallography_measurement.diffrn_id (key)


               The data item is a pointer to _diffrn.id in the DIFFRN
               category.



#### _pdbx_serial_crystallography_measurement.focal_spot_size


            The focal spot size of the beam
            impinging on the sample (micrometres squared).



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_measurement.photons_per_pulse


               The photons per pulse measured in  (tera photons (10^(12)^)/pulse units).



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_measurement.pulse_duration


               The average duration (femtoseconds)
	       of the pulse energy measured at the sample.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_measurement.pulse_energy


               The energy/pulse of the X-ray pulse impacting the sample measured in microjoules.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_measurement.pulse_photon_energy


              The photon energy of the X-ray pulse measured in KeV.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_measurement.source_distance


               The distance from source to the sample along the optical axis (metres).



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_measurement.source_size


               The dimension of the source beam measured at the source (micrometres squared).



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_measurement.xfel_pulse_repetition_rate


               For FEL experiments, the pulse repetition rate measured in cycles per seconds.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


## Category pdbx_serial_crystallography_sample_delivery


               Data items in the PDBX_SERIAL_CRYSTALLOGRAPHY_SAMPLE_DELIVERY category
               record general details about the sample delivery

---


```
     
         Example 1
     
         _pdbx_serial_crystallography_sample_delivery.diffrn_id   1
         _pdbx_serial_crystallography_sample_delivery.description 'LCP injector'
     
```


---

| Attribute | Key | Required | Type | Units | Enumerated | Bounded |
| --------- | --- | -------- | ---- | ----- | ---------- | ------- |
| description | no | no | text | None | no | no |
| diffrn_id | yes | yes | code | None | no | no |
| method | no | yes | text | None | yes | no |

---

#### _pdbx_serial_crystallography_sample_delivery.description


               The description of the mechanism by which the specimen in placed in the path
               of the source.



#### _pdbx_serial_crystallography_sample_delivery.diffrn_id (key)


               The data item is a pointer to _diffrn.id in the DIFFRN
               category.



#### _pdbx_serial_crystallography_sample_delivery.method (required)


               The description of the mechanism by which the specimen in placed in the path
               of the source.



---

| Allowed Values | Detail |
| -------------- | ------ |
| fixed target |   |
| injection |   |


## Category pdbx_serial_crystallography_sample_delivery_fixed_target


               Data items in the PDBX_SERIAL_CRYSTALLOGRAPHY_SAMPLE_DELIVERY_FIXED_TARGET
               category record details about sample delivery using a fixed taget.

---


```
     
         Example 1
     
         _pdbx_serial_crystallography_sample_delivery_fixed_target.diffrn_id          1
         _pdbx_serial_crystallography_sample_delivery_fixed_target.sample_holding     mesh
         _pdbx_serial_crystallography_sample_delivery_fixed_target.support_base       goniometer
         _pdbx_serial_crystallography_sample_delivery_fixed_target.crystals_per_unit  7
```


---

| Attribute | Key | Required | Type | Units | Enumerated | Bounded |
| --------- | --- | -------- | ---- | ----- | ---------- | ------- |
| crystals_per_unit | no | no | int | None | no | yes |
| description | no | no | text | None | no | no |
| details | no | no | text | None | no | no |
| diffrn_id | yes | yes | code | None | no | no |
| motion_control | no | no | line | None | no | no |
| sample_dehydration_prevention | no | no | line | None | no | no |
| sample_holding | no | no | text | None | no | no |
| sample_solvent | no | no | text | None | no | no |
| sample_unit_size | no | no | float | micrometres | no | yes |
| support_base | no | no | text | None | no | no |
| velocity_horizontal | no | no | float | None | no | yes |
| velocity_vertical | no | no | float | None | no | yes |

---

#### _pdbx_serial_crystallography_sample_delivery_fixed_target.crystals_per_unit


               The number of crystals per dropplet or pore in fixed target



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_sample_delivery_fixed_target.description


               For a fixed target sample, a description of sample preparation



#### _pdbx_serial_crystallography_sample_delivery_fixed_target.details


               Any details pertinent to the fixed sample target



#### _pdbx_serial_crystallography_sample_delivery_fixed_target.diffrn_id (key)


               The data item is a pointer to _diffrn.id in the DIFFRN
               category.



#### _pdbx_serial_crystallography_sample_delivery_fixed_target.motion_control


               Device used to control movement of the fixed sample



#### _pdbx_serial_crystallography_sample_delivery_fixed_target.sample_dehydration_prevention


               Method to prevent dehydration of sample



#### _pdbx_serial_crystallography_sample_delivery_fixed_target.sample_holding


               For a fixed target sample, mechanism to hold sample in the beam



#### _pdbx_serial_crystallography_sample_delivery_fixed_target.sample_solvent


               The sample solution content and concentration



#### _pdbx_serial_crystallography_sample_delivery_fixed_target.sample_unit_size


               Size of pore in grid supporting sample. Diameter or length in micrometres,
               e.g. pore diameter



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_sample_delivery_fixed_target.support_base


               Type of base holding the support



#### _pdbx_serial_crystallography_sample_delivery_fixed_target.velocity_horizontal


               Velocity of sample horizontally relative to a perpendicular beam in millimetres/second



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_sample_delivery_fixed_target.velocity_vertical


               Velocity of sample vertically relative to a perpendicular beam in millimetres/second



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


## Category pdbx_serial_crystallography_sample_delivery_injection


               Data items in the PDBX_SERIAL_CRYSTALLOGRAPHY_SAMPLE_DELIVERY_INJECTION
               category record details about sample delivery by injection

---


```
     
         Example 1
     
         _pdbx_serial_crystallography_sample_delivery_injection.diffrn_id               1
         _pdbx_serial_crystallography_sample_delivery_injection.description             'microextrusion injector'
         _pdbx_serial_crystallography_sample_delivery_injection.injector_diameter       50
         _pdbx_serial_crystallography_sample_delivery_injection.flow_rate               0.22
         _pdbx_serial_crystallography_sample_delivery_injection.carrier_solvent         'liquid'
```


---

| Attribute | Key | Required | Type | Units | Enumerated | Bounded |
| --------- | --- | -------- | ---- | ----- | ---------- | ------- |
| carrier_solvent | no | no | text | None | no | no |
| crystal_concentration | no | no | float | None | no | yes |
| description | no | no | text | None | no | no |
| diffrn_id | yes | yes | code | None | no | no |
| filter_size | no | no | float | micrometres | no | yes |
| flow_rate | no | no | float | microliters_per_min | no | yes |
| injector_diameter | no | no | float | micrometres | no | yes |
| injector_nozzle | no | no | text | None | no | no |
| injector_pressure | no | no | float | kilopascals | no | yes |
| injector_temperature | no | no | float | kelvins | no | yes |
| jet_diameter | no | no | float | micrometres | no | yes |
| power_by | no | no | text | None | no | no |
| preparation | no | no | text | None | no | no |

---

#### _pdbx_serial_crystallography_sample_delivery_injection.carrier_solvent


               For continuous sample flow experiments, the carrier buffer used
               to move the sample into the beam. Should include protein
               concentration.



#### _pdbx_serial_crystallography_sample_delivery_injection.crystal_concentration


               For continuous sample flow experiments, the concentration of
               crystals in the solution being injected.

               The concentration is measured in million crystals/ml.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_sample_delivery_injection.description


               For continuous sample flow experiments, a description of the injector used
               to move the sample into the beam.



#### _pdbx_serial_crystallography_sample_delivery_injection.diffrn_id (key)


               The data item is a pointer to _diffrn.id in the DIFFRN
               category.



#### _pdbx_serial_crystallography_sample_delivery_injection.filter_size


               The size of filter in micrometres in filtering crystals



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_sample_delivery_injection.flow_rate


               For continuous sample flow experiments, the flow rate of
               solution being injected  measured in ul/min.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_sample_delivery_injection.injector_diameter


               For continuous sample flow experiments, the diameter of the
               injector in micrometres.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_sample_delivery_injection.injector_nozzle


               The type of nozzle to deliver and focus sample jet



#### _pdbx_serial_crystallography_sample_delivery_injection.injector_pressure


               For continuous sample flow experiments, the mean pressure
               in kilopascals at which the sample is injected into the beam.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_sample_delivery_injection.injector_temperature


               For continuous sample flow experiments, the temperature in
               Kelvins of the speciman injected. This may be different from
               the temperature of the sample.



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 100.0 | 370.0 |


#### _pdbx_serial_crystallography_sample_delivery_injection.jet_diameter


               Diameter in micrometres of jet stream of sample delivery



---

| Minimum&nbsp;Value | Maximum&nbsp;Value |
| ------------- | ------ |
| 0.0 | <h3>+&infin;</h3> |


#### _pdbx_serial_crystallography_sample_delivery_injection.power_by


               Sample deliver driving force, e.g. Gas, Electronic Potential



#### _pdbx_serial_crystallography_sample_delivery_injection.preparation


               Details of crystal growth and preparation of the crystals


