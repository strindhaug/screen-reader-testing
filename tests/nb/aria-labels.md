
<div lang="nb">

# Aria-label testing

Det virker som om det er noe rart i TalkBack, i allefall med React at den insisterer på å fokusere på de innerste taggene og leser en og en tagg eller linje i kildekoden (uavhengig av setningsstruktur). Og å ha aria-label på en wrapper rundt dette hjelper ikke siden den bare hopper over dette og leser de indre taggene.

Dette er en test på flere varianter av wrappere med aria-label for å se hvilke som virker i en statisk HTML sammenheng.

<p aria-label="50 kroner per stykk, 120 kroner per kilo">
    <strong>50 kr</strong>
    <i>
        120 kr/kg
    </i>
</p>

<p aria-label="50 kroner per stykk, 120 kroner per kilo">
    <strong aria-hidden="true">50 kr</strong>
    <i aria-hidden="true">120 kr/kg</i>
</p>


<p>
    <strong aria-label="50 kroner per stykk, 120 kroner per kilo">50 kr</strong>
    <i aria-hidden="true">120 kr/kg</i>
</p>

</div>
