# omarchy-efexx-theme

Tema pessoal do efexx para [Omarchy](https://omarchy.org). Paleta Matrix/cyberpunk dark.

**Cores principais:**
- Background: `#080E0A` (verde-preto)
- Foreground: `#c8f7d8` (branco-gelo verde)
- Accent: `#39FF14` (verde elétrico Matrix)

---

## Instalação

```bash
omarchy theme install https://github.com/efexx/omarchy-efexx-theme
omarchy theme set efexx
```

Após instalar, definir o wallpaper padrão:

```bash
omarchy theme bg set ~/.config/omarchy/themes/efexx/backgrounds/Arch14.png
```

---

## Texto da waybar

O tema define `foreground = #c8f7d8` para o terminal. Na waybar, adicionar esta linha após o `@import` em `~/.config/waybar/style.css` para usar o cinza-lavanda do Tokyo Night:

```css
@define-color foreground #a9b1d6;
```

---

## Customização

Edite `colors.toml` para alterar a paleta. O Omarchy regenera automaticamente as configs do terminal, Hyprlock, Mako, btop, etc.

| Variável | Cor atual | Uso |
|---|---|---|
| `background` | `#080E0A` | Fundo de janelas e barra |
| `foreground` | `#c8f7d8` | Texto principal (terminal) |
| `accent` | `#39FF14` | Bordas ativas, cursor, destaques |
| `color1` | `#50f872` | Verde vivo |
| `color6` | `#7cf8f7` | Ciano brilhante |

---

## Arquivos do tema

| Arquivo | Descrição |
|---|---|
| `colors.toml` | Paleta principal (obrigatório) |
| `btop.theme` | Cores do monitor de sistema btop |
| `icons.theme` | Tema de ícones do sistema |
| `neovim.lua` | Cores do Neovim |
| `vscode.json` | Tema para VS Code / Code OSS |
| `backgrounds/` | 18 wallpapers Arch Linux |
| `preview.png` | Screenshot do desktop |
| `unlock.png` | Screenshot da tela de bloqueio |

---

## O que este tema NÃO inclui

Estas configs ficam no RESTORE_GUIDE.md:

- Layout e módulos do Waybar (`config.jsonc`)
- Scripts de bateria BTTL (`omarchy-bttl-battery`)
- Keybindings, touchpad, gestos
- Fingerprint / PAM
- Voxtype
- Launchers de IA rápida (Super+Q, Super+')
- Calendário popup (gsimplecal)
- Volume control (pavucontrol)
