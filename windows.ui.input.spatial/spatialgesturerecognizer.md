---
-api-id: T:Windows.UI.Input.Spatial.SpatialGestureRecognizer
-api-type: winrt class
---

<!-- Class syntax.
public class SpatialGestureRecognizer : Windows.UI.Input.Spatial.ISpatialGestureRecognizer
-->

# Windows.UI.Input.Spatial.SpatialGestureRecognizer

## -description
Interprets user interactions from hands, controllers, and system voice commands to surface spatial gesture events, which users target using their gaze.

## -remarks
Spatial gestures are a key form of input for HoloLens. By routing interactions from the [SpatialInteractionManager](spatialinteractionmanager.md) to a hologram's [SpatialGestureRecognizer](spatialgesturerecognizer.md), apps can detect Tap, Hold, Manipulation, and Navigation events uniformly across hands, voice, and controllers.

[SpatialGestureRecognizer](spatialgesturerecognizer.md) performs only the minimal disambiguation between the set of gestures that you request. For example, if you request just Tap, the user may hold their finger down as long as they like and a Tap will still occur. If you request both Tap and Hold, after about a second of holding down their finger, the gesture will promote to a Hold and a Tap will no longer occur.

To use [SpatialGestureRecognizer](spatialgesturerecognizer.md) , handle the [SpatialInteractionManager](spatialinteractionmanager.md) 's InteractionDetected event and grab the SpatialPointerPose exposed there. Use the user's gaze ray from this pose to intersect with the holograms and surface meshes in the user's surroundings, in order to determine what the user is intending to interact with. Then, route the SpatialInteraction in the event arguments to the target hologram's [SpatialGestureRecognizer](spatialgesturerecognizer.md) , using its CaptureInteraction method. This starts interpreting that interaction according to the SpatialGestureSettings set on that recognizer at creation time or by TrySetGestureSettings.

On HoloLens, interactions and gestures should generally derive their targeting from the user's gaze, rather than trying to render or interact at the hand's location directly. Once an interaction has started, relative motions of the hand may be used to control the gesture, as with the Manipulation or Navigation gesture.

## -examples

## -see-also
