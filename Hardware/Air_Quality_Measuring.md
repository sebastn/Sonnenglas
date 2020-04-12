# Air Quality Index

There are two types of AQIs and they are entirely different:
 - Indoor AQI
   - CO
   - Volatile organic compounds (VOCs)
   - Radon
   - NO2
   - Secondhand smoke, also called environmental tobacco smoke
   - Lead particles
   - Asbestos
   - CO2
 - Outdoor AQI
   - PM
   - Sulfur dioxide (SO2)
   - Carbon monoxide (CO)
   - Nitrogen dioxide (NO2)
   - Ozone (O3)

The criteria for measuring Indoor AQI and Outdoor AQI are different.

Now, regarding the significance of CO2 in Air Quality Index, let's look at the definition of a pollutant first:
``` To be defined as a pollutant, the substance has to “cause or contribute to air pollution which may reasonably be anticipated to endanger public health or welfare".```

CO2 is not strictly defined as a pollutant as it is plays a significant role in preserving life on earth. So we can say that **CO2** content in the air is not necessarily a representation of the Air Quality.

However, it's indeed a harmful gas and with regard to indoor AQ, exceeding the nominal limits of CO2 concentration indoors can result in discomforts.

### Indoor AQI
 Indoor air quality (IAQ) is the air quality within and around buildings and structures and  it relates especially to the health and comfort of building occupants. it is affected by a number of things. Before we move on to IAQI measurement, we will list out the common indoor air pollutants: (https://goo.gl/mzWohb)
  - CO
  - Volatile organic compounds (VOCs)
  - Radon
  - NO2
  - Secondhand smoke, also called environmental tobacco smoke
  - Lead particles
  - Asbestos
  - CO2

 There are two opinions about measuring indoor air quality:
 - concentration of VOCs and CO (namely the above mentioned pollutants) is the indicating factor
 - concentration of CO2 is the indicating factor of Air Quality

## For CO2 Measurement
Although CO2 is not considered as a factor for measuring indoor AQI, the logic that **Netatmo** might have followed is that, higher level of CO2 inside a room can cause discomfort, headache and it affects decision making and cognition of humans. CO2 levels in a room or an enclosed space increase due to human occupancy and human respiration. So concentration of indoor CO2 level is a direct function of human occupancy and ventilation. The main drawback is that although they track the CO2 put out by people, they don’t detect any dangerous chemicals and we can't assess the associated health risks. Ideally, along with the CO2 sensor, you should have a radon detector and a carbon monoxide detector in your home as well.

## Against CO2 Measurement
On the other hand, measurement of the above mentioned pollutants give us the Indoor AQI and most of the indoor AQ Sensors measure those values. To measure indoor air quality you need a special tool called a **VOC** sensor which measures volatile organic compounds. It can pick up the **formaldehyde** that’s present in new carpets as well as the **ketones** that come from people filling a space.

# Conclusion
Because of the above mentioned reasons, I believe that spending 20$ on a CO2 sensor (which gives only CO2 concentration) is not wise as we need additional components like radon detector and CO detector to make a sensible measurement of AQ.

On the other hand, the low cost AQ sensors mainly measure VOCs and CO by default. My personal suggestion is the CCS811 sensor($7.25) or CCS801 sensor ($4.44) from 'AMS' and it measures
- Volatile Organic Compounds (VOCs)
- equivalent total VOC (eTVOC)
- equivalent CO2 (eCO2) values
