paper-chip
==========
Material Design: [Chips](thttp://www.google.com/design/spec/components/chips.html)

`paper-chip` is a small element represents a complex entity such as a calendar
event or a contact. The chip can be in an opened (active) or closed (inactive)
state. In its closed state, it contains an icon and a short title. In its open
state, the chip expands to show more detail about the represented entity, as
well as (optionally) a "remove" button that removes the chip element from the
DOM.

The following child elements may be placed within the chip tag define its
content:

  * `.icon`: The icon representing the chip. This may be any element, for
             example, a `<core-icon>` or a simple `<span>` with a single letter
  * `h1`: The chip label, shown in both closed and opened states
  * `h2`: A secondary label, shown only in the opened state

The `removable` attribute can be used to add a button which removes the chip
from teh DOM.

## Examples:

Removable chip with core-icon

    <paper-chip removable>
      <core-icon class="icon" icon="avatars:avatar-1"></core-icon>
      <h1>John Doe</h1>
      <h2>jdoe@example.com</h2>
    </paper-chip>

Basic chip with single letter instead of an icon

    <paper-chip label="Jane Doe">
      <div class="icon" flex>J</div>
      <h1>jdoe@example.com</h1>
    </paper-chip>

