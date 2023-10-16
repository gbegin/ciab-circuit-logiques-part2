---
title: Conception d'un circuit séquentiel synchrone
---


# Conception d'un circuit séquentiel synchrone

Concevoir un circuit logique séquentiel permet de répondre à un besoin
pratique qui ne peut pas être satisfait par un circuit combinatoire.
Le point de départ est une description, la plus précise possible, du
besoin à satisfaire: quelles doivent être la ou les entrées, 
sorties ou conditions qui font passer d'un état au suivant,
etc. Pour un besoin donné, une multitude de solutions
fonctionnellement équivalentes sont possibles; ainsi, il faudra établir
des critères ou identifier des contraintes qui permettront d'orienter
la conception et le choix final d'une solution. Deux systèmes peuvent
avoir un même comportement vu de l'extérieur, mais comporter des
nombres d'états internes différents.

Des considérations pratiques nous amèneront souvent à vouloir réduire
le nombre d'états nécessaires, et à simplifier les différents circuits
combinatoires utilisés. Réduire le nombre de bascules utilisées ne se
traduit pas toujours par un système plus simple, car les décodeurs
d'état et de sortie peuvent alors s'en trouver plus complexes.


## Spécification fonctionnelle

Comme dans tout problème de conception, la formulation en mots de la
spécification du système est cruciale. Appliquer parfaitement une
procédure de conception en se basant sur une spécification erronée ne
peut pas conduire à un système adéquat.

Il faudra un bon bagage d'expérience et d'intuition au concepteur ou à
la conceptrice pour
pouvoir interpréter  une description
informelle, très souvent  incomplète, ambiguë et
imprécise, et la traduire
correctement en un design concret qui répond à un besoin maladroitement
exprimé. Il revient à cette personne de s'assurer que ce qu'elle a compris
correspond bien à ce qui était demandé.

La première question à poser est: *Que doit faire le système?* Suivront
d'autres questions, amenant à définir davantage de détails: *Doit-il y avoir des entrées? Si oui, combien? Combien de
sorties sont nécessaires?* Le comportement du système pourra être
essentiellement caractérisé en répondant à la question: *Quelle doit
être la séquence des sorties, pour une certaine séquence d'entrées?*
Mais comme les séquences d'entrées peuvent être en nombre infini, il
faudra identifier des patrons qui permettront de résumer le
comportement du système.
