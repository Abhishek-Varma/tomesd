# Changelog


## v0.1
 - **[2023.03.30]** Initial release.
 - **[2023.03.31]** Added support for more resolutions than multiples of 16. (Fixes #8)
 - **[2023.03.31]** Added support for diffusers (thanks @JunnYu and @ExponentialML)! (Fixes #1)

## v0.1.1
 - **[2023.04.01]** Rewrote how the model patching works to address some compatibility issues (e.g., ControlNet). (Fixes #9)

## v0.1.2
 - **[2023.04.03]** Added support for MPS devices (i.e., M1/M2 Macs). Thanks @brkirch! (Fixes #4)
   - **Note:** This fix still isn't perfect and may require some extra changes.
 - **[2023.04.04]** `use_rand` now forces itself off if the batch size is odd (meaning the prompted and unprompted images arent in the same batch). This should fix some artifacting without needing to tinker with the settings.