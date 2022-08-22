# State diagram

```mermaid
stateDiagram
[*] --> app_boilerplate
state app_boilerplate {
[*] --> load
load --> instal
instal --> Theme
state Theme {
[*] --> theme
theme --> new_theme
theme --> our_theme
new_theme --> create
our_theme --> choose
create --> connect_theme
choose --> connect_theme
connect_theme --> Website
state Website {
[*] --> website
website --> assembly
assembly --> [*]
    }
  }
}

