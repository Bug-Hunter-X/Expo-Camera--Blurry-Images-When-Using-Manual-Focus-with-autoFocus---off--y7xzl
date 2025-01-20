# Expo Camera Focus Issue

This repository demonstrates a bug in the Expo Camera API related to inconsistent focusing behavior when using manual focus with `autoFocus` set to 'off'.

## Bug Description

When `autoFocus` is set to 'off' and `setFocusDepth` is used for manual focusing, the captured images are sometimes blurry even when the preview appears to be in focus. This inconsistency makes reliable manual focusing challenging.

## Reproduction Steps

1. Clone this repository.
2. Run the app using `expo start`.
3. Observe that images captured with `setFocusDepth` may be blurry despite the preview appearing sharp.

## Potential Solution

The proposed solution involves a workaround that attempts to address the focus inconsistency by delaying the image capture after setting the focus depth. 

## Note
This issue is intermittent. The blurriness is not always reproducible, which makes debugging more difficult. 