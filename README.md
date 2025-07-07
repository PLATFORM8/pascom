# pascom

Example Asterisk action script for dialing with a custom CLIP number.

This repository contains `clip_action_script.conf`, a dialplan snippet
that allows users to set an outbound caller ID by entering a code
followed by the desired CLIP number and destination.

## Usage

Dial a number in the following format:

```
#123*<clip-number>*<destination>
```

For example:

```
#123*015127652445*012340123456789
```

The script parses the number between the first pair of `*` characters
(`015127652445` in the example) and uses it as the caller ID before
calling the final destination.

See `clip_action_script.conf` for the actual dialplan script.
