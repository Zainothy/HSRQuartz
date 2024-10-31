---
Topic: Data Representation
---
Sound is made up of bits that are stored in files on a computer. Well.. digital sound is. 

>[!info] Sampling 
>Sound is sampled, to then be stored digitally: 
>- Sound is recorded as an analogue signal by a microphone. **Analogue signals are pieces of data, that are continually changing** 
>- Before computers can read analogue signals, they need to be converted into digital data so that it can be read and stored 
>	- This is done through analogue to digital converters, found in most modern recording devices 
>	  
><mark class="hltr-pink">This conversion process is called sampling</mark>

## Sampling In Depth: 

To convert analogue recording to digital data, amplitude of a soundwave is sampled at regular intervals. The amplitude has limited values that are dependent on the bit depth. 

Once a device samples a recording, it creates a digital curve. In this curve, each block of data matches where a sample was taken. 

The data can be improved by taking samples more regularly, this is known as having a higher **Sample Rate**. 

--- 

```chartsview
#-----------------#
#- chart type    -#
#-----------------#
type: Column

#-----------------#
#- chart data    -#
#-----------------#
data:
  - Time: "0"
    "Time ": 10
  - Time: "1"
    "Time ": 50
  - Time: "2"
    "Time ": 70
  - Time: "3"
    "Time ": 60
  - Time: "4"
    "Time ": 70
  - Time: "5"
    "Time ": 90
  - Time: "6"
    "Time ": 120
  - Time: "7"
    "Time ": 70
  - Time: "8"
    "Time ": 50
  - Time: "9"
    "Time ": 30
  - Time: "10"
    "Time ": 20
  - Time: "11"
    "Time ": 10
  - Time: "12"
    "Time ": 1
  - Time: "13"
    "Time ": 1
  - Time: "14"
    "Time ": 50
  - Time: "15"
    "Time ": 70
  - Time: "16"
    "Time ": 71
  - Time: "17"
    "Time ": 40
  - Time: "18"
    "Time ": 30
  - Time: "19"
    "Time ": 20
  - Time: "20"
    "Time ": 0
  - Time: ""

#-----------------#
#- chart options -#
#-----------------#
options:
  xField: Time
  yField: "Time "
```

## Quality of Sound Files: 

There are many things that affect the quality of a sound file, some include: 
- **Sample Rate**: Also known as sampling frequency, is the number of samples per second, typically measured in hertz or khz. A common sample rate is 44.1kHz 
- **Bit Depth:** The number of bits available during each sample. 
	- Increasing sample rate means the analogue recording is sampled more often, this will improve quality 
	- Increasing bit depth, will increase the threshold for the volume of sounds that will be picked up, even if they are happening simultaneously to louder ones. This will result in a sampled sound more close to the original recording 
- **Increasing either of these will always increase file size: keep this in mind** 
