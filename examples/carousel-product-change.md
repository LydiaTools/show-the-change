# Example: a change you can see

This example was written by applying the skill's instructions to [Aspectory's public v0.2.0 change](https://github.com/LydiaTools/aspectory/commit/e749fd51e4e3bfed4e673a951964b2bb2b18aa96), its [release notes](https://github.com/LydiaTools/aspectory/releases/tag/v0.2.0), and its recorded checks. It is not an independent model evaluation.

**What changed for you:** You can put landscape, square and portrait photos into the same carousel frame without cropping the displayed image. The tool can export a numbered ZIP, keeping the order you chose. The original graphic composer remains available.

**Where to look:** Open [Carousel Fit](https://lydiatools.github.io/aspectory/carousel.html?lang=en). Choose **Try a sample set**, select **4:5**, and look at the three previews. Use the arrows to reorder them, then choose **Download PNG ZIP**. The built-in examples are synthetic; you can also add your own PNG, JPEG or WebP images.

**What was checked:** The v0.2.0 release reports 13 Node tests and a local Chrome check of export sizes, image corners, ordering and offline export. A later [CI run](https://github.com/LydiaTools/aspectory/actions/runs/40088687278) also checked three separately credited CC0 practice photos. These are recorded checks, not evidence that someone published a successful campaign.

![Actual Carousel Fit interface with three differently shaped practice photos in matching 4:5 frames.](https://raw.githubusercontent.com/LydiaTools/aspectory/c8293abbc337aacd733cae5ef0a19607995fa951/docs/screenshots/carousel-photos-en.jpg)

*Actual application screenshot from the later CC0 photo example, not the built-in synthetic sample. The full downloaded inputs are kept in frame through resampling. [Photo credits and screenshot provenance](https://github.com/LydiaTools/aspectory/blob/c8293abbc337aacd733cae5ef0a19607995fa951/docs/screenshots/PROVENANCE.md). The screenshot was added after the fixed v0.2.0 release.*

**What remains to check:** The release notes do not claim physical-phone or Safari testing. Preview your exports on the destination platform; the feature prepares a common frame and does not publish for you. The prior checks were on October 24, 2026; they are not a fresh test of your device.
