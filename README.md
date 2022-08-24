
-...
- ..
$.ajax({
  method: "POST",
  url: "https://avatar.roblox.com/v1/avatar/thumbnail-customization",
  contentType: "application/json",
  data: JSON.stringify({
    "camera": {
        // Ranges are inclusive.
        "distanceScale": 2, // 0.5 to 4 - Camera distance scale from the avatar
        "fieldOfViewDeg": 30, // 15 to 45 - Camera Field Of View (FOV) in degrees, slight effect
        "xRotDeg": 0, // -20 to 20 - Camera X rotation in degrees
        // !!!!! Roblox **might** remove this field soon:
        "yRotDeg": 0 // -60 to 60 - Camera Y rotation in degrees
    },
    "emoteAssetId": 0, /* The assetId of an emote you own. 0 for no emote. 
    * example: 3696763549 in https://www.roblox.com/catalog/3696763549/Heisman-Pose
    */
    // idleAnimationAssetId used to exist here, it has since been removed.
    "thumbnailType": 1 /* The thumbnailType
    * 1 = Closeup (headshot)
    * 2 = FullBody (bodyshot)
    
    Closeup and Fullbody can have separate configurations.
    */
  })
})
// 
<!---
pablo109/pablo109 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
