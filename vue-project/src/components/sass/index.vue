<template>
    <div>
        <a href="https://sass-lang.com/documentation" target="_blank">Dokumentacja scss</a>
    </div>
    <!-- <l1-zmienne></l1-zmienne> -->
    <!-- <l2_zmienne_part2></l2_zmienne_part2> -->
    <!-- <l3_listy></l3_listy> -->
    <!-- <l4_domieszki></l4_domieszki> -->
    <!-- <l5_zagniezdzanie></l5_zagniezdzanie> -->
    <!-- <l6_domieszki-zparametrami></l6_domieszki-zparametrami> -->
    <!-- <l7_funkcje></l7_funkcje> -->
    <!-- <l8_zagniezdzanie_pseudoklas></l8_zagniezdzanie_pseudoklas> -->
    <!-- <l9_tworzenie_nazw_za_pomoca_ampersand></l9_tworzenie_nazw_za_pomoca_ampersand> -->
    <!-- <l10_pseudoklasa_extend_i_placeholder></l10_pseudoklasa_extend_i_placeholder> -->
    <!-- <l11_import_i_kompilacja_plikow></l11_import_i_kompilacja_plikow> -->
    <!-- <l12_instrukcja_warunkowa_if></l12_instrukcja_warunkowa_if> -->
    <!-- <l13_petla_for></l13_petla_for> -->
    <!-- <l14_petla_each></l14_petla_each> -->
    <!-- <l15_petla_while></l15_petla_while> -->
    <l16_funkcje_wbudowane></l16_funkcje_wbudowane>
</template>

<script>
import l10_pseudoklasa_extend_i_placeholder from './l10_pseudoklasa_extend_i_placeholder.vue';
import l11_import_i_kompilacja_plikow from './l11_import_i_kompilacja_pilkow/l11_import_i_kompilacja_plikow.vue';
import l12_instrukcja_warunkowa_if from './l12_instrukcja_warunkowa_if.vue';
import l13_petla_for from './l13_petla_for.vue';
import l14_petla_each from './l14_petla_each.vue';
import l15_petla_while from './l15_petla_while.vue';
import l16_funkcje_wbudowane from '@/components/sass/l16_funkcje_wbudowane.vue';

import l1Zmienne from './l1_zmienne.vue';
import l2_zmienne_part2 from './l2_zmienne_part2.vue';
import l3_listy from './l3_listy.vue';
import l4_domieszki from './l4_domieszki.vue';
import l5_zagniezdzanie from './l5_zagniezdzanie.vue';
import L6_domieszkiZparametrami from './l6_domieszkiZparametrami.vue';
import l7_funkcje from './l7_funkcje.vue';
import l8_zagniezdzanie_pseudoklas from './l8_zagniezdzanie_pseudoklas.vue';
import l9_tworzenie_nazw_za_pomoca_ampersand from './l9_tworzenie_nazw_za_pomoca_ampersand.vue';


export default {
    components: {
        l1Zmienne,
        l2_zmienne_part2,
        l3_listy,
        l4_domieszki,
        l5_zagniezdzanie, 
        L6_domieszkiZparametrami,
        l7_funkcje,
        l8_zagniezdzanie_pseudoklas,
        l9_tworzenie_nazw_za_pomoca_ampersand,
        l10_pseudoklasa_extend_i_placeholder,
        l11_import_i_kompilacja_plikow,
        l12_instrukcja_warunkowa_if,
        l13_petla_for,
        l14_petla_each,
        l15_petla_while,
        l16_funkcje_wbudowane
    }
}
</script>