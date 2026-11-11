# Delta FastFlags

Just fflags from delta listed here, no reliable source was found so.

**These are still working.**

```lua
--[[ DebugDisplayFPS
 Shows an FPS counter overlay on screen. ]]
setfflag("DebugDisplayFPS", "true")

--[[ TaskSchedulerTargetFps
 Caps the render framerate. 10 = 10 FPS cap. ]]
setfflag("TaskSchedulerTargetFps", "10")

--[[ DebugFRMQualityLevelOverride
 Overrides the graphics quality slider. 1 = minimum quality, 21 = max. ]]
setfflag("DebugFRMQualityLevelOverride", "1")

--[[ FRMMaxGrassDistance
 Maximum render distance for grass. 0 = disable grass entirely. ]]
setfflag("FRMMaxGrassDistance", "0")

--[[ FRMMinGrassDistance
 Minimum distance before grass starts rendering. 0 = starts exactly where you are. ]]
setfflag("FRMMinGrassDistance", "0")

--[[ DebugForceMSAASamples
 Forces MSAA anti-aliasing. 1, 2, or 4 samples. 4 = smoothest edges. ]]
setfflag("DebugForceMSAASamples", "4")

--[[ RobloxGuiBlurIntensity
 Blur strength on menus / loading screens. 0 = no blur. ]]
setfflag("RobloxGuiBlurIntensity", "0")

--[[ DebugSkyGray
 Replaces the skybox with flat gray. ]]
setfflag("DebugSkyGray", "true")

--[[ DebugPauseVoxelizer
 Stops terrain voxelization, can freeze terrain updates. ]]
setfflag("DebugPauseVoxelizer", "true")

--[[ GrassMovementReducedMotionFactor
 Reduces grass sway animation. 1 = enabled. ]]
setfflag("GrassMovementReducedMotionFactor", "1")

--[[ CSGLevelOfDetailSwitchingDistance
 Distance at which CSG models drop to low LOD. 1 = aggressive. ]]
setfflag("CSGLevelOfDetailSwitchingDistance", "1")

--[[ CSGLevelOfDetailSwitchingDistanceL12
 LOD switch distance for tier 1→2 detail. 0 = always high detail. ]]
setfflag("CSGLevelOfDetailSwitchingDistanceL12", "0")

--[[ CSGLevelOfDetailSwitchingDistanceL23
 LOD switch distance for tier 2→3 detail. 0 = always high detail. ]]
setfflag("CSGLevelOfDetailSwitchingDistanceL23", "0")

--[[ CSGLevelOfDetailSwitchingDistanceL34
 LOD switch distance for tier 3→4 detail. 0 = always high detail. ]]
setfflag("CSGLevelOfDetailSwitchingDistanceL34", "0")

--[[ FastGPULightCulling3
 Faster GPU-side light culling. Generally an FPS win. ]]
setfflag("FastGPULightCulling3", "true")

--[[ RenderGpuTextureCompressor
 Enables GPU-side texture compression. ]]
setfflag("RenderGpuTextureCompressor", "true")

--[[ DebugRenderingSetDeterministic
 Forces deterministic render order, debugging aid. ]]
setfflag("DebugRenderingSetDeterministic", "true")

--[[ GraphicsGLEnableSuperHQShadersExclusion
 Excludes super-high-quality shaders on OpenGL. ]]
setfflag("GraphicsGLEnableSuperHQShadersExclusion", "false")

--[[ GraphicsGLEnableHQShadersExclusion
 Excludes high-quality shaders on OpenGL. ]]
setfflag("GraphicsGLEnableHQShadersExclusion", "false")

--[[ GraphicsCheckComputeSupport
 Enables compute shader support check at startup. ]]
setfflag("GraphicsCheckComputeSupport", "true")

--[[ RenderShadowmapBias
 Shadow map bias. 0 = default; raise to remove shadow acne. ]]
setfflag("RenderShadowmapBias", "0")

--[[ DebugDontRenderUI
 Stops rendering the entire UI. Huge FPS win, breaks interaction. ]]
setfflag("DebugDontRenderUI", "false")

--[[ DebugDontRenderScreenGui
 Stops rendering ScreenGui instances. ]]
setfflag("DebugDontRenderScreenGui", "false")

--[[ DebugAdornsDisabled
 Hides selection boxes and adorns. ]]
setfflag("DebugAdornsDisabled", "false")

--[[ DebugGraphicsPreferVulkan
 Forces the Vulkan renderer on Android. Can be a big perf gain. ]]
setfflag("DebugGraphicsPreferVulkan", "true")

--[[ DebugGraphicsPreferOpenGL
 Forces the OpenGL ES renderer on Android. Fallback if Vulkan crashes. ]]
setfflag("DebugGraphicsPreferOpenGL", "false")

--[[ DebugGraphicsPreferD3D11
 Forces Direct3D 11. ]]
setfflag("DebugGraphicsPreferD3D11", "false")

--[[ TaskSchedulerAutoThreadLimit
 Caps the automatic worker thread count. Lower = less stutter sometimes. ]]
setfflag("TaskSchedulerAutoThreadLimit", "8")

--[[ DebugRunParallelLuaOnMainThread
 Runs parallel Lua on the main thread instead of workers. ]]
setfflag("DebugRunParallelLuaOnMainThread", "false")

--[[ DebugPerfMode
 Internal performance mode toggle. Exact effect undocumented. ]]
setfflag("DebugPerfMode", "true")

--[[ DefaultMeshCacheSizeMB
 Base mesh cache size in megabytes. ]]
setfflag("DefaultMeshCacheSizeMB", "256")

--[[ MeshContentProviderForceCacheSize
 Forces mesh cache to a fixed byte size. 0 = no force. ]]
setfflag("MeshContentProviderForceCacheSize", "0")

--[[ UserIdPlayerNameCacheSize
 Cache for user-id → username lookups, in bytes. ]]
setfflag("UserIdPlayerNameCacheSize", "33554432")

--[[ EmotesAnimationsPerPlayerCacheSize
 Per-player emote animation cache in bytes. ]]
setfflag("EmotesAnimationsPerPlayerCacheSize", "16777216")

--[[ S2PhysicsSenderRate
 Physics network send rate per second. 0 = stop sending (solo FPS gain, multiplayer desync). ]]
setfflag("S2PhysicsSenderRate", "0")

--[[ ConnectionMTUSize
 Network packet MTU in bytes. Changing can disconnect you. ]]
setfflag("ConnectionMTUSize", "900")

--[[ MaximumUnstickForceInGs
 Maximum unstick force. Negative = wallglide / fling behavior. ]]
setfflag("MaximumUnstickForceInGs", "-1000")

--[[ MinClientSimulationRadius
 Minimum network ownership radius. Huge = simulate everything locally. ]]
setfflag("MinClientSimulationRadius", "2147000000")

--[[ MaxClientSimulationRadius
 Maximum network ownership radius. Pair with MinClientSimulationRadius. ]]
setfflag("MaxClientSimulationRadius", "2147000000")

--[[ DebugUseCustomSimRadius
 Required to be true for Min/MaxClientSimulationRadius to apply. ]]
setfflag("DebugUseCustomSimRadius", "true")

--[[ CameraMaxZoomDistance
 Maximum camera zoom-out distance in studs. ]]
setfflag("CameraMaxZoomDistance", "99999")

--[[ ScrollWheelDeltaAmount
 Scroll wheel sensitivity multiplier. ]]
setfflag("ScrollWheelDeltaAmount", "1")

--[[ FontSizePadding
 Extra padding around UI text. ]]
setfflag("FontSizePadding", "3")

--[[ EnableInGameMenuChrome
 Enables the new in-game menu chrome. ]]
setfflag("EnableInGameMenuChrome", "true")

--[[ EnableInGameMenuModernization
 Enables the modernized in-game menu layout. ]]
setfflag("EnableInGameMenuModernization", "true")

--[[ EnableCameraByDefault
 Starts with camera enabled by default. ]]
setfflag("EnableCameraByDefault", "false")

--[[ EnableQuickGameLaunch
 Enables the fast game launch path. ]]
setfflag("EnableQuickGameLaunch", "false")

--[[ VoiceBetaBadge
 Shows or hides the voice chat beta badge. ]]
setfflag("VoiceBetaBadge", "false")

--[[ CanHideGuiGroupId
 Group ID whose GUI elements can be hidden. Leave unless you know the ID. ]]
setfflag("CanHideGuiGroupId", "32380007")

--[[ TrackMacWebLaunchFlow
 Tracks mac web launch flow. ]]
setfflag("TrackMacWebLaunchFlow", "false")

--[[ DisableDPIScale
 Disables DPI scaling, UI will render at native pixel size. ]]
setfflag("DisableDPIScale", "true")

--[[ EnableBubbleChatFromChatService
 Enables bubble chat driven by ChatService. ]]
setfflag("EnableBubbleChatFromChatService", "true")

--[[ DebugForceChatDisabled
 Forces chat to be disabled. Set false to leave chat alone. ]]
setfflag("DebugForceChatDisabled", "false")

-- These are supported but have no visible effect

setfflag("CrashUploadToBacktracePercentage", "0")
setfflag("CrashReportingHundredthsPercentage", "0")
setfflag("EphemeralCounterInfluxReportingEnabled", "false")
setfflag("ClientLightingTechnologyChangedTelemetryHundredthsPercent", "0")
setfflag("BootstrapperTelemetryReportingHundredthsPercentage", "0")
setfflag("LinkBrowserTrackerToDeviceRollout", "0")
setfflag("BrowserTrackerIdTelemetryEnabled", "false")
setfflag("LocServicePerformanceAnalyticsEnabled", "false")
setfflag("StartupTracingInfluxRollout", "0")
setfflag("VideoCaptureServiceEnabled", "false")
setfflag("PredictedOOM", "false")
setfflag("PredictedOOMPercent", "0")
setfflag("HttpCurlConnectionCacheSize", "0")
setfflag("ReportDeviceInfoRollout", "0")
setfflag("TerrainOTAMaxTextureSize", "1024")
setfflag("AnimationClipMemCacheEnabled", "true")
setfflag("HSRClusterSymmetryDistancePercent", "10000")
setfflag("LmsClientRollout2", "0")
setfflag("V1MenuLanguageSelectionFeaturePerMillageRollout", "0")
setfflag("AvatarChatServiceUserPermissionsAudioEligible", "false")
setfflag("FacialAnimationStreamingServiceUniverseSettingsEnableAudio", "false")
setfflag("FacialAnimationStreamingServiceUserSettingsOptInAudio", "false")
setfflag("FacialAnimationStreamingServiceUserSettingsOptInVideo", "false")
setfflag("VoiceChatServiceManagerUseAvatarChat", "false")
```
