---
weight: 10
---

# Projecting at Conferences Using OBS Streaming Software

Generally, in conference venues with 50-100 or more participants, streaming software is used to project materials.
As a projection method for such conferences, we will introduce how to project xBridge using the streaming software [OBS](https://obsproject.com/).
With projection, you can display subtitle results transparently together with presentation materials like PowerPoint, as shown in the photo below.

{{< figure src="images/screen-with-obs.png" class="center" >}}

{{< hint info >}}
**Screen Projection Translation Mode is also available**  
This guide is created using the screen projection subtitle mode described in [Joining a meeting as a viewer (screen projection subtitle mode)]({{< relref "/docs/conversation/join-conversation-screen-subtitle" >}}), but you can use the same operations in translation mode as well.
{{< /hint >}}

## 1. Prepare Hardware Equipment

### 1-2. Prepare Venue Hardware Equipment

The hardware equipment configuration to be used is as follows.
Projection from the streaming PC to the screen varies by venue, so please adjust accordingly.

{{< figure src="images/hardware-architecture.png" class="center" >}}

| Hardware                     | Overview                                                                                                                                                                                               |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Host PC                      | Accesses xBridge and operates as a host to start and end meetings. Also simultaneously accesses xBridge as a speaker and inputs audio to distribute interpretation to participants.                 |
| Audio Interface              | Used to input audio from the venue to the host PC via microphone. Not necessary if the microphone is directly connected to the host PC, but for conferences, audio input is separated to distribute to multiple sources. |
| WiFi for Host PC             | WiFi for the host PC. Please isolate from participant communications and ensure stable internet connection.                                                                                            |
| Streaming PC                 | The streaming PC that operates what is projected on the venue screen. Generally managed using streaming software. This guide uses OBS.                                                               |
| Extended Display for Streaming PC | An extended display to check the screen of materials being projected.                                                                                                                              |

### 1-2. Host PC Setup

Please set up the host PC by referring to [Basic PC configuration for hosts]({{< relref "/docs/other/pc-basic-configuration" >}}).

## 2. Meeting Creation and Setup

### 2-1. Create a Meeting as Host

Please create a meeting by referring to the guide [Creating a meeting]({{< relref "/docs/conversation/create-conversation" >}}).

### 2-2. Start a Meeting as Host

Next, open a browser (Google Chrome) and start the meeting as a host.
For how to start a meeting, please refer to the guide [Starting a meeting]({{< relref "/docs/conversation/start-conversation" >}}).

### 2-3. Join the Meeting as a Speaker

Next, open a new tab in the host PC's browser and join the meeting as a speaker.
For how to join a meeting, please refer to the guide [Joining a meeting as a speaker]({{< relref "/docs/conversation/join-conversation-speaker" >}}).
If the speaker's language changes during the meeting, please exit once, select the language again, and rejoin.

{{< hint danger >}}
**Please maintain the meeting in a started state as the host**  
During the meeting, never close the tab where the host is participating and maintain the meeting in a started state.
If the host leaves the meeting, other participants will be forcibly removed.
{{< /hint >}}

## 3. Design Adjustment for Screen Projection

On the streaming PC, join the meeting and adjust the screen design by referring to the guide ["Display Settings" in Joining a meeting as a viewer (screen projection subtitle mode)]({{< relref "/docs/conversation/join-conversation-screen-subtitle/#表示設定をする" >}}).
After adjustment, press the `CREATE AND COPY` button for `Shared Link (Fullscreen Mode)` to copy the shared link.

{{< figure src="images/screen-design.png" title="Design sample. Displays the latest 3 messages with large font size." class="center" >}}

## 4. Projection with OBS Streaming Software

### 4-1. Install OBS Streaming Software

Please install OBS on the streaming PC for the day of the event.
The installer can be downloaded from [Download OBS Studio](https://obsproject.com/ja/download).

### 4-2. Add Sources to Project in OBS

From Windows `System` `Display`, select `Extend these displays` and set the connected display as an extended screen.
If you are using PowerPoint, please switch to presentation mode and confirm that the screen is displayed on the extended display.

{{< figure src="images/windows-extended-screen.png" class="center" >}}

{{< hint warning >}}
**Projection is also possible with windows instead of extended screens.**  
This guide describes projecting materials to an extended display connected to the PC main unit and streaming the entire screen.
If an extended display cannot be arranged, you can display PowerPoint materials in window mode in presentation mode and project it using OBS's `Window Capture` function.
However, in this case, a status bar will be displayed at the bottom of PowerPoint.
{{< /hint >}}

Open OBS and click to add a source from the `+` button in `Sources`.

{{< figure src="images/obs-1-add-source.png" class="center" >}}

Select `Display Capture`.

{{< figure src="images/obs-add-screen-capture.png" class="center" width="150" >}}

Select the extended display where materials are being projected. (Example: DELL S2421H)

{{< figure src="images/obs-select-screen-capture-window.png" class="center" >}}

### 4-3. Add xBridge as a Source in OBS

Open OBS and click to add a source from the `+` button in `Sources`.
Select `Browser`.

{{< figure src="images/obs-add-browser.png" class="center" width="150" >}}

Add the `Shared Link (Fullscreen Mode)` copied in step [3. Design Adjustment for Screen Projection]({{< relref "/docs/usecase/conference-screen/#3スクリーン投影のデザイン調整" >}}) to the `URL` in OBS browser settings.
Please set other items such as `Width` and `Height` according to your environment.

{{< figure src="images/obs-browser-xbridge.png" class="center" >}}

### 4-4. OBS Source Layout Adjustment

Please adjust the size of the two added sources to match the projection screen.

{{< figure src="images/obs-layout-design.png" class="center" >}}

### 4-5. OBS Projection to Screen

To output to the connected HDMI screen, right-click the layout at the top of the screen and select the screen to project from `Fullscreen Projector (Preview)`.
For other streaming destinations, please see the [OBS help page](https://obsproject.com/help).

{{< figure src="images/obs-output-preview.png" class="center" >}}

## 5. Venue Preparation/Day of Event Proceedings

### 5-1. Venue Preparation

- [ ] To enable users to use xBridge on smartphones at any time, we recommend electronically distributing participant viewer links via email or other means.
- [ ] To enable users to use xBridge on smartphones at any time, attach QR codes for participant viewers at the venue.

### 5-2. Day of Event Proceedings

- [ ] On the day of the event, during OBS projection, the meeting host must keep the meeting in a started state.
- [ ] We recommend that the host start the meeting 15 minutes before the session begins on the day of the event so that users can enter.
