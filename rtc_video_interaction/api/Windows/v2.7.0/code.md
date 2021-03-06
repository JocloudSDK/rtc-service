# Error code

## ThunderRet

| Error code | Meaning |
| :--- | :--- |
| THUNDER_RET_SUCCESS(0) | Processing succeeded |
| THUNDER_RET_NOT_INITIALIZED(-1) | Not initialized |
| THUNDER_RET_WRONG_INIT_STATUS(-2) | A wrong initialization status. Before the initialization or destroying is finished, this error will be returned when an interface is called. |
| THUNDER_RET_NO_JOIN_ROOM(-3) | Not joining a room [Before joining a room, this error will be returned only if an interface called before joining a room is called] |
| THUNDER_RET_ALREADY_JOIN_ROOM(-4) | Already joining a room [After joining a room, this error will be returned only if an interface called before joining a room is called] |
| THUNDER_RET_WRONG_JOIN_STATUS(-5) | A wrong joining status. Before room joining or room quitting is finished, this error will be returned when this interface is called. |
| THUNDER_RET_NOT_IN_THUNDER(-6) | Not in a Thunder mode (This error will be returned only if an interface called by Thunder is called in a ThunderBolt mode) |
| THUNDER_RET_NOT_IN_THUNDERBOLT(-7) | Not in a ThunderBolt mode (This error will be returned only if an interface called by ThunderBolt is called in a Thunder mode) |
| THUNDER_RET_INVALID_UID(-8) | Invalid uid |
| THUNDER_RET_INVALID_ROOMID(-9) | Invalid room id |
| THUNDER_RET_INVALID_URL(-10) | Invalid url |
| THUNDER_RET_INVALID_TASKID(-11) | Invalid task id |
| THUNDER_RET_CAPACITY_LIMIT(-12) | SDK capacity limit (super-threshold of a stream publishing address) |
| THUNDER_RET_INVALID_ARGUMENT(-13) | Invalid parameters (when necessary parameters are null or illegal) |
| THUNDER_RET_START_AUDIO_CAPTURE_ERR(-14) | Error in starting audio capture |
| THUNDER_RET_NO_START_AUDIO_CAPTURE(-15) | Not starting audio capture. In the case of not enabling capture, this error will be returned when external data is pushed. |
| THUNDER_RET_ALREADY_START_AUDIO_CAPTURE(-16) | Already starting audio capture. This error will be returned when resetting is executed during capturing. |
| THUNDER_RET_NO_START_AUDIO_PUBLISH(-17) | Not starting audio publishing. In the case of not starting publishing, this error will be returned when external data is pushed. |
| THUNDER_RET_ALREADY_START_AUDIO_ENCODE(-18) | Already starting audio capture. This error will be returned when resetting is executed during capturing. |
| THUNDER_RET_ALREADY_START_AUDIO_PUBLISH(-19) | Audio publishing has been enabled, repeating publish setting will return this error code |
| THUNDER_RET_NOT_ON_FRONT_CAMERA(-20) | This error will be returned if a camera mirror is set on a rear camera. |
| THUNDER_RET_NOT_ON_MULTI_TYPE(-21) | When a multi-user microphone connection layout is set, this error will be returned if a remote play type is set before users join a room. |
| THUNDER_RET_INVALID_SEATINDEX(-22) | This error will be returned when the preset seat number for multi-user microphone connection exceeds a layout setting range. |
| THUNDER_RET_INVALID_TRANSCODING_MODE(101) | Invalid transcoding mode |
| THUNDER_NOTIFY_JOIN_FAIL(-2001) | Notifying that room joining fails when SDK does not receive services due to network (SDK will execute room quitting operation if the room joining fails) |
| THUNDER_RET_AUDIO_ENGINE_ERROR(-3001) | Returning an audio engine error. It is required to check logs for specific reasons. |
| THUNDER_RET_AUDIO_DISABLE_VOICE_POSITION(-3002) | Not enabling voice stereo of remote users. |
| THUNDER_RET_VIDEO_ENGINE_ERROR(-4001) | Returning a video engine error. It is required to check logs for specific reasons. |
| THUNDER_RET_TRANS_ENGINE_ERROR(-5001) | Returning a transfer engine error. It is required to check logs for specific reasons. |
| THUNDER_RET_ARGO_ENGINE_ERROR(-6001) | Returning a configuration engine error. It is required to check logs for specific reasons. |
| THUNDER_RET_SERVICE_ENGINE_ERROR(-7001) | Returning a SERVICE engine error. It is required to check logs for specific reasons. |
| THUNDER_RET_LOG_ENGINE_ERROR(-8001) | Returning a LOG engine error. It is required to check logs for specific reasons. |