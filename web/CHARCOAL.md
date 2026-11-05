# Charcoal viewer chrome

The CSS variables mirror android-NDK's charcoal contract at
3e682fb1175beef5625dbd2418730220e49fc9bd. The existing page layout, native browser
controls, finite evaluators, shader inputs and actual Wegert phase colors stay
unchanged. Ordinary primary/secondary text uses F4/B4 against 21/2F/38 roles;
focus and selection are explicit, and disabled controls use the exempt 85 role.

The existing opt-in browser smoke reads the real computed root, surface, control
and text colors. It temporarily makes the root white, requires rejection, then
restores the original state before screenshots. This code executes only under
the existing smoke query; it adds no production initialization work. Existing
WebGL readback and independent numerical agreement checks remain mandatory.

Browser execution and actual screenshots are required before visual acceptance.
They prove neither Android nor physical phone execution. This branch contains no
current Android host: the standalone GLES interface remains source-only. No page
deployment, release or installation is performed.
