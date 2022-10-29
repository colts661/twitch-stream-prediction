# Twitch Stream Watch Prediction
Huy Trinh, Yacun Wang<br>
December 2021

### Data
Please download the data from [this Google Drive link](https://drive.google.com/drive/folders/1BD8m7a8m7onaifZay05yYjaLxyVV40si?usp=sharing) and place them inside the `data` directory.

#### Description

The full version of stream data is from the paper:

**Recommendation on Live-Streaming Platforms: Dynamic Availability and Repeat Consumption**<br>
Jérémie Rappaz, Julian McAuley and Karl Aberer<br>
*RecSys*, 2021

This is a dataset of users consuming streaming content on Twitch. The full version retrieved all streamers, and all users connected in their respective chats, every 10 minutes during 43 days.

Due to hardware constraints, the project used the 100k benchmark dataset.

#### Statistics
|             | 100k        | full     |
| ----------- | ----------- | ---      |
| Users       | 100K        | 15.5M    |
| Streamers   | 162.6K      | 465K     |
| Interactions| 3M          | 124M     |
| Time Steps  | 6148        | 6148     |

#### Metadata
Start and stop times are provided as integers and represent periods of 10 minutes. Stream ID could be used to retrieve a single broadcast segment from a streamer (not used in our work).
* User ID (anonymized)
* Stream ID
* Streamer username
* Time start
* Time stop

#### Example
```
    1,34347669376,grimnax,5415,5419
    1,34391109664,jtgtv,5869,5870
    1,34395247264,towshun,5898,5899
    1,34405646144,mithrain,6024,6025
    2,33848559952,chfhdtpgus1,206,207
    2,33881429664,sal_gu,519,524
    2,33921292016,chfhdtpgus1,922,924
```