---

layout: ribbon

style: |

    #Cover img, #Conclusion img {
      width: 100%;
      height: 100%;
    }
    #Cover h2 {
        display: none;
        }
    #Conclusion h2 {
      position: absolute;
      top: 2px;
      left: 2px;
    }
    #Cover p, #Conclusion p {
        margin:10px 0 0;
        text-align:center;
        color:#FFF;
        font-style:italic;
        font-size:20px;
        }
        #Cover p a {
            color:#FFF;
            }
    p.mycover, p.mycover img {
      width: 100%;
      height: 100%;
    }
    p.h {
      margin-bottom: 10px;
    }
    .w img {
      width: 100%;
    }
    .h img {
      height: 100%;
    }
---

# Ivre, il oublie de lancer sa commande dans tmux {#Cover}

![](pictures/ivre-cover.png)

## Terminal Multiplexer

- Dæmon permettant de créer des sessions groupant plusieurs fenêtres shell
- Possibilité de se « détacher » d'une session pour s'y réattacher plus tard.

## Intérêt d'un multiplexeur de terminal

- Lancer une commande longue sans peur des pertes de connexion ;
- Garder des shells ouverts, faciles à récupérer ;
- Travailler à 4 mains/yeux à distance ;
- Ne pas lancer ssh à chaque fois qu'on veut un nouveau shell sur le serveur ;
- Pouvoir scroller facilement en TTY.

// Garder un shell ouvert même en cas de déconnexion

## Tmux

- http://tmux.github.io/
- Depuis Juillet 2007
- Licence BSD

## vs Screen

- Plus léger ;
- Meilleure gestion des sessions ;
- Status bar plus facile à configurer ;
- Beaucoup plus facile à scripter.

// Sessions gérées par un processus serveur unique VS chaque session a son serveur.

## Usage de base (+démo)

- tmux
- tmux a / attach-session
- tmux new-session -s foobar
- tmux attach -t foobar
- Se déplacer dans tmux

## Usage avancé (+démo)

- Copy mode & Paste
- Fun with panes
- Scripting a bit
- More fun with panes

## Pour finir

- On ne lance pas de backup dans tmux #TitreMensonger
- Nommez vos sessions
- Germinal : un terminal ultra léger utilisant tmux

## ![](pictures/bhtmux-cartoon.jpg) {#Conclusion}
