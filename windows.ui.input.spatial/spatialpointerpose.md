---
-api-id: T:Windows.UI.Input.Spatial.SpatialPointerPose
-api-type: winrt class
-api-device-family-note: xbox
---

<!-- Class syntax.
public class SpatialPointerPose : Windows.UI.Input.Spatial.ISpatialPointerPose, Windows.UI.Input.Spatial.ISpatialPointerPose2
-->

# Windows.UI.Input.Spatial.SpatialPointerPose

## -description
Represents the available spatial pointing poses, such as the user's head gaze and each spatial controller's pointing pose, for use in targeting hand gestures, spatial controller presses, and voice interactions.

## -remarks
The SpatialPointingPose provides the set of pointing rays available at the time represented by the [Timestamp](spatialpointerpose_timestamp.md) property.

When targeting a spatial interaction, such as a hand gesture, spatial controller press or voice interaction, apps should choose a pointing ray available from the interaction's SpatialPointerPose, based on the nature of the interaction's [SpatialInteractionSource](spatialinteractionsource.md):
* If the interaction source does not support pointing ([IsPointingSupported](spatialinteractionsource_ispointingsupported.md) is false), the app should target based on the user's gaze, available through the [Head](spatialpointerpose_head.md) property.
* If the interaction source does support pointing ([IsPointingSupported](spatialinteractionsource_ispointingsupported.md) is true), the app may instead target based on the source's pointing pose, available through the [TryGetInteractionSourcePose](spatialpointerpose_trygetinteractionsourcepose_1162732260.md) method.

The app should then intersect the chosen pointing ray with its own holograms or with the spatial mapping mesh to render cursors and determine what the user is intending to interact with.

Once an interaction has started, relative motions of the hand or controller may be used to control the gesture, as with the [Manipulation](spatialgesturerecognizer_gesturesettings.md) or [Navigation](spatialgesturerecognizer_gesturesettings.md) gesture.

## -examples

## -see-also
