# Category Group xfel_group


              Categories that describe X-ray Free Electron Laser (XFEL) data collection and experimental details.

---

## Category pdbx_xfel_data_reduction


               Data items in the PDBX_XFEL_DATA_REDUCTION category record
               details about data processing that are unique to XFEL experiments.
               These will compliment data recorded in category pdbx_diffrn_merge_stat.

---


```
     
         Example 1
     
         _pdbx_xfel_data_reduction.diffrn_id           1
         _pdbx_xfel_data_reduction.frames_total        7324430
         _pdbx_xfel_data_reduction.frames_hits         1797503
         _pdbx_xfel_data_reduction.frames_indexed      578620
```


---

| Attribute | Key | Required | Type | Units | Enumerated | Bounded |
| --------- | --- | -------- | ---- | ----- | ---------- | ------- |
| diffrn_id | yes | yes | code | None | no | no |
| frames_failed_index | no | no | int | None | no | no |
| frames_hits | no | no | int | None | no | no |
| frames_indexed | no | no | int | None | no | no |
| frames_total | no | no | int | None | no | no |
| pulse_events | no | no | int | None | no | no |
| run_numbers | no | no | text | None | no | no |

---

#### _pdbx_xfel_data_reduction.diffrn_id (key)


               The data item is a pointer to _diffrn.id in the DIFFRN
               category.



#### _pdbx_xfel_data_reduction.frames_failed_index


            For experiments in which samples are provided in a
            continuous stream, the total number of data frames collected
            that contained a "hit" but failed to index.



#### _pdbx_xfel_data_reduction.frames_hits


            For experiments in which samples are provided in a
            continuous stream, the total number of data frames collected
            in which the sample was hit.



#### _pdbx_xfel_data_reduction.frames_indexed


            For experiments in which samples are provided in a
            continuous stream, the total number of data frames collected
            that were indexed.



#### _pdbx_xfel_data_reduction.frames_total


            The total number of data frames collected for this
            data set.



#### _pdbx_xfel_data_reduction.pulse_events


            For FEL experiments, the number of pulse events in the dataset.



#### _pdbx_xfel_data_reduction.run_numbers


               For data collection using different batches,
               indicates which subset of the data collected
               were used in producing this dataset.



## Category pdbx_xfel_detector


               Data items in the PDBX_XFEL_DETECTOR category record
               details the detector used in the experiment

---


```
     
         Example 1
     
         _pdbx_xfel_detector.diffrn_id     1
         _pdbx_xfel_detector.type          'CS-PAD CXI-1'
         _pdbx_xfel_detector.detector      'PIXEL ARRAY DETECTOR'
         _pdbx_xfel_detector.frequency     120
```


---

| Attribute | Key | Required | Type | Units | Enumerated | Bounded |
| --------- | --- | -------- | ---- | ----- | ---------- | ------- |
| details | no | no | text | None | no | no |
| detector | no | yes | line | None | yes | no |
| diffrn_id | yes | yes | code | None | no | no |
| frequency | no | no | text | None | no | no |
| type | no | yes | line | None | yes | no |

---

#### _pdbx_xfel_detector.details


               A description of special aspects of the radiation detector.



#### _pdbx_xfel_detector.detector (required)


               The class of detector used for data collection



---

| Allowed Values | Detail |
| -------------- | ------ |
| CCD |   |
| CMOS |   |
| PIXEL ARRAY DETECTOR |   |


#### _pdbx_xfel_detector.diffrn_id (key)


               The data item is a pointer to _diffrn.id in the DIFFRN
               category.



#### _pdbx_xfel_detector.frequency


               The frequency of the detector (Hz) used in data collection.



#### _pdbx_xfel_detector.type (required)


               The type of detector used for data collection



---

| Allowed Values | Detail |
| -------------- | ------ |
| CS-PAD CXI-1 |   |
| CS-PAD CXI-2 |   |
| CS-PAD XPP |   |
| CUSTOM-MADE |   |
| RAYONIX MX-325 |   |
| RAYONIX MX170-HS |   |
| RAYONIX MX325HE |   |
| RAYONIX SX-165mm |   |


## Category pdbx_xfel_measurement


               Data items in the PDBX_XFEL_MEASUREMENT category record
               details the beam that is impinging on the sample

---


```
     
         Example 1
     
         _pdbx_xfel_measurement.diffrn_id                1
         _pdbx_xfel_measurement.pulse_duration           45
         _pdbx_xfel_measurement.photons_per_pulse        .17
         _pdbx_xfel_measurement.focal_spot_size          1.8
         _pdbx_xfel_measurement.collection_time_total   61036
```


---

| Attribute | Key | Required | Type | Units | Enumerated | Bounded |
| --------- | --- | -------- | ---- | ----- | ---------- | ------- |
| collection_time_total | no | no | float | seconds | no | no |
| collimation | no | no | text | None | no | no |
| diffrn_id | yes | yes | code | None | no | no |
| focal_spot_size | no | no | float | micrometres_squared | no | no |
| photons_per_pulse | no | no | float | teraphotons_per_pulse | no | no |
| pulse_duration | no | no | float | femtoseconds | no | no |
| pulse_energy | no | no | float | microjoules | no | no |
| pulse_photon_energy | no | no | float | kiloelectron_volts | no | no |
| pulse_repetition_rate | no | no | float | hertz | no | no |
| source_distance | no | no | float | metres | no | no |
| source_size | no | no | float | micrometres_squared | no | no |

---

#### _pdbx_xfel_measurement.collection_time_total


            The total number of seconds required to measure this data set.



#### _pdbx_xfel_measurement.collimation


               The collimation or type of focusing optics applied to the radiation.



#### _pdbx_xfel_measurement.diffrn_id (key)


               The data item is a pointer to _diffrn.id in the DIFFRN
               category.



#### _pdbx_xfel_measurement.focal_spot_size


            Focal spot size of the beam impinging on the sample (micrometres squared).



#### _pdbx_xfel_measurement.photons_per_pulse


               The photons per pulse measured in  (tera photons (10^(12)^)/pulse units).



#### _pdbx_xfel_measurement.pulse_duration


               Average duration (femtoseconds) of the pulse energy
               measured at the sample.



#### _pdbx_xfel_measurement.pulse_energy


               The energy/pulse of the X-ray pulse impacting the sample measured in microjoules.



#### _pdbx_xfel_measurement.pulse_photon_energy


               The photon energy of the X-ray pulse measured in KeV.



#### _pdbx_xfel_measurement.pulse_repetition_rate


               The pulse repetition rate measured in cycles per seconds.



#### _pdbx_xfel_measurement.source_distance


               The distance from source to the sample along the optical axis (metres).



#### _pdbx_xfel_measurement.source_size


               The dimension of the source beam measured at the source (micrometres squared).



## Category pdbx_xfel_sample_delivery


               Data items in the PDBX_XFEL_SAMPLE_DELIVERY category
               record general details about XFEL the sample delivery

---


```
     
         Example 1
     
         _pdbx_xfel_sample_delivery.diffrn_id   1
         _pdbx_xfel_sample_delivery.description 'LCP injector'
     
```


---

| Attribute | Key | Required | Type | Units | Enumerated | Bounded |
| --------- | --- | -------- | ---- | ----- | ---------- | ------- |
| description | no | yes | text | None | no | no |
| diffrn_id | yes | yes | code | None | no | no |

---

#### _pdbx_xfel_sample_delivery.description (required)


               The description of the mechanism by which the specimen in placed in the path
               of the source.



#### _pdbx_xfel_sample_delivery.diffrn_id (key)


               The data item is a pointer to _diffrn.id in the DIFFRN
               category.



## Category pdbx_xfel_sample_delivery_injection


               Data items in the PDBX_XFEL_SAMPLE_DELIVERY_INJECTION
               category record details about sample delivery by injection

---


```
     
         Example 1
     
         _pdbx_xfel_sample_delivery_injection.diffrn_id               1
         _pdbx_xfel_sample_delivery_injection.description             'microextrusion injector'
         _pdbx_xfel_sample_delivery_injection.injector_diameter       50
         _pdbx_xfel_sample_delivery_injection.flow_rate               0.22
         _pdbx_xfel_sample_delivery_injection.carrier_solvent         'Crystallization bufer with 7.9 MAG'
```


---

| Attribute | Key | Required | Type | Units | Enumerated | Bounded |
| --------- | --- | -------- | ---- | ----- | ---------- | ------- |
| carrier_solvent | no | no | text | None | no | no |
| description | no | no | text | None | no | no |
| diffrn_id | yes | yes | code | None | no | no |
| flow_rate | no | no | float | microliters_per_min | no | no |
| injector_diameter | no | no | float | micrometres | no | no |
| injector_pressure | no | no | float | kilopascals | no | no |
| injector_temperature | no | no | float | kelvins | no | no |
| preparation | no | no | text | None | no | no |
| sample_concentration | no | no | float | None | no | no |

---

#### _pdbx_xfel_sample_delivery_injection.carrier_solvent


               For continuous sample flow experiments, the carrier buffer used
               to move the sample into the beam. Should include protein
               concentration.



#### _pdbx_xfel_sample_delivery_injection.description


               For continuous sample flow experiments, a description of the injector used
               to move the sample into the beam.



#### _pdbx_xfel_sample_delivery_injection.diffrn_id (key)


               The data item is a pointer to _diffrn.id in the DIFFRN
               category.



#### _pdbx_xfel_sample_delivery_injection.flow_rate


               For continuous sample flow experiments, the flow rate of
               solution being injected  measured in ul/min.



#### _pdbx_xfel_sample_delivery_injection.injector_diameter


               For continuous sample flow experiments, the diameter of the
               injector in micrometres.



#### _pdbx_xfel_sample_delivery_injection.injector_pressure


               For continuous sample flow experiments, the mean pressure
               in kilopascals at which the sample is injected into the beam.



#### _pdbx_xfel_sample_delivery_injection.injector_temperature


               For continuous sample flow experiments, the temperature in
               Kelvins of the speciman injected. This may be different from
               the temperature of the sample.



#### _pdbx_xfel_sample_delivery_injection.preparation


               Details of crystal growth and preparation of the crystals



#### _pdbx_xfel_sample_delivery_injection.sample_concentration


               For continuous sample flow experiments, the concentration of
               crystals in the solution being injected.

               The concentration is measured in million crystals/ml.



## Category pdbx_xfel_source


               Data items in the PDBX_XFEL_SOURCE category record
               details about the source used in the experiment

---


```
     
         Example 1
     
         _pdbx_xfel_source.diffrn_id       1
         _pdbx_xfel_source.site            'SLAC LCLS'
         _pdbx_xfel_source.site_beamline   'SLAC LCLS BEAMLINE CXI (SC1)'
```


---

| Attribute | Key | Required | Type | Units | Enumerated | Bounded |
| --------- | --- | -------- | ---- | ----- | ---------- | ------- |
| diffrn_id | yes | yes | code | None | no | no |
| site | no | yes | line | None | yes | no |
| site_beamline | no | yes | line | None | yes | no |

---

#### _pdbx_xfel_source.diffrn_id (key)


               The data item is a pointer to _diffrn.id in the DIFFRN
               category.



#### _pdbx_xfel_source.site (required)


               The site of the free electron laser (FEL) source.



---

| Allowed Values | Detail |
| -------------- | ------ |
| SACLA |   |
| SLAC LCLS |   |


#### _pdbx_xfel_source.site_beamline (required)


              The Free Electron Laser (FEL) facility, beamline and sample chamber identification.



---

| Allowed Values | Detail |
| -------------- | ------ |
| SACLA BEAMLINE BL3 |   |
| SLAC LCLS BEAMLINE CXI (SC01) |   |
| SLAC LCLS BEAMLINE CXI (SC1) |   |
| SLAC LCLS BEAMLINE CXI (SC2) |   |
| SLAC LCLS BEAMLINE MFX |   |
| SLAC LCLS BEAMLINE XPP |   |

