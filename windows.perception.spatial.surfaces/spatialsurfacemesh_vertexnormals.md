---
-api-id: P:Windows.Perception.Spatial.Surfaces.SpatialSurfaceMesh.VertexNormals
-api-type: winrt property
---

<!-- Property syntax
public Windows.Perception.Spatial.Surfaces.SpatialSurfaceMeshBuffer VertexNormals { get; }
-->

# Windows.Perception.Spatial.Surfaces.SpatialSurfaceMesh.VertexNormals

## -description
Gets the buffer object representing the mesh's normal buffer, if IncludeVertexNormals was set as a mesh option in the call to SpatialSurfaceInfo.TryComputeLatestMeshAsync. Otherwise, this property is null.

## -property-value
The mesh buffer if available; otherwise null.

## -remarks
If the SpatialSurfaceMeshOptions.VertexNormalFormat option is also set, this buffer will be generated in the format indicated.

## -examples

## -see-also
