---
-api-id: M:Windows.Graphics.Holographic.HolographicCameraRenderingParameters.SetFocusPoint(Windows.Perception.Spatial.SpatialCoordinateSystem,Windows.Foundation.Numerics.Vector3)
-api-type: winrt method
---

<!-- Method syntax
public void SetFocusPoint(Windows.Perception.Spatial.SpatialCoordinateSystem coordinateSystem, Windows.Foundation.Numerics.Vector3 position)
-->

# Windows.Graphics.Holographic.HolographicCameraRenderingParameters.SetFocusPoint

## -description
Sets the stationary point in the holographic space that the user will likely focus on for the current frame.

This is used to improve image quality at the focus point and along a default focus plane that faces the user.

You must set the focus point each frame, or it will reset to its default.

## -parameters
### -param coordinateSystem
The coordinate system of the position vector.

### -param position
The location of the focus point in the specified coordinate system.

## -remarks

## -examples

## -see-also
[SetFocusPoint(SpatialCoordinateSystem, Vector3, Vector3)](holographiccamerarenderingparameters_setfocuspoint_1275160748.md), [SetFocusPoint(SpatialCoordinateSystem, Vector3, Vector3, Vector3)](holographiccamerarenderingparameters_setfocuspoint_1040378076.md)