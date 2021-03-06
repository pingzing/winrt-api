---
-api-id: P:Windows.ApplicationModel.VoiceCommands.VoiceCommandResponse.MaxSupportedVoiceCommandContentTiles
-api-type: winrt property
---

<!-- Property syntax
public uint MaxSupportedVoiceCommandContentTiles { get; }
-->

# Windows.ApplicationModel.VoiceCommands.VoiceCommandResponse.MaxSupportedVoiceCommandContentTiles

## -description
Gets the maximum number of content tiles the background app service can display on the **Cortana** canvas.

## -property-value
The maximum number of content tiles.

## -remarks
The maximum number of tiles that can be displayed depends on the feedback screen being shown. One item when the [VoiceCommandResponse](voicecommandresponse.md) is created for [ReportProgressAsync](voicecommandserviceconnection_reportprogressasync.md) or [RequestConfirmationAsync](voicecommandserviceconnection_requestconfirmationasync.md), and more than one item when the [VoiceCommandResponse](voicecommandresponse.md) is created for [RequestDisambiguationAsync](voicecommandserviceconnection_requestdisambiguationasync.md).

## -examples

## -see-also
[ elements and attributes v1.2](https://docs.microsoft.com/en-us/uwp/schemas/voicecommands/voice-command-elements-and-attributes-1-2.md), [Cortana interactions](http://msdn.microsoft.com/library/4c11a7cf-da26-4ca1-a9b9-fe52670101f5), [Cortana design guidelines](http://msdn.microsoft.com/library/a92c084b-9913-4718-9a04-569d51ace55d), [Cortana voice command sample](http://go.microsoft.com/fwlink/p/?LinkID=619899)