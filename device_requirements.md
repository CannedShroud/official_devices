Device Requirements


The device MUST be using an ARM 64-bit software base. ARM 32-bit devices are no longer supported from our side.

The device MUST have SELinux Enforcing to release builds. During Beta Stage builds it's allowed to have SELinux Permissive.

The device MUST have complete hardware compatibility corresponding to the stock ROM, i.e. if IR blaster works on the stock ROM, it must work on Lighthouse. Only VoLTE is allowed to be ignored, so are NFC payment methods.

The device MUST NOT include any unused overlays and packages. This includes, but is not limited to, packages not being built, packages that don't work, obsolete packages, placebo 'tweaks' or any packages that will include unnecessary and/or unwanted features, as stated at the Maintainers Code of Conduct.

The device sources MUST be in accordance with, if applicable, all the items stated at our Maintainers Code of Conduct related to the device source code.


The device MUST NOT have the need for a lot of patches, and if so, it must be in accordance with the following listing below.

If there are commits that are needed in repos other than the device-specific ones, they MUST:

Be necessary for the device to build, boot, or even to have a/the device's function(s) working properly (e.g. Fingerprint On Display).

Have proper authorship.

Be as minimal and polished as possible.

Be in accordance with the items, if applicable, stated at our Maintainers Code of Conduct.

All the trees should be posted and public on Github/Gitlab.At the time of applying, we compare them with different other repos from other developers/projects to check if things like authorship and commit history are on point. 
 
Sources should not have more than 3 (three) branches with other Custom ROM projects.As much as we like to have people building and sharing the great work of other projects, we need dedicated people who might want to test some new things or check if everything is on point, not buildbots who are constantly making 69 builds for the sake of a developer title.

Respect authorship and make your forks. Having your custom device tree guarantees that if something is broken, you can fix it fast. Dumb thing to clarify at this point. So, it's better if you do your forks with the whole adapting to our ROM instead of linking us some Lineage/Other developer trees (the only exception to this rule is kernel/vendor trees that requires little to no changes most of the time) that you used to build. Also, sources without proper commit authorship or "Initial commit" (the 1 commit magic device tree) sources will be completely ignored.