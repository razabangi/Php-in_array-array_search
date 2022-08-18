<?php

// Topic:
// in_array and array_search

// ================= in_array | in_array returns true or false only

// $array = ['blue', 'green', 'orange', 'black', 'red'];
// if (in_array('blue', $array)) {
//     echo "Yes";
// } else {
//     echo "No";
// }
// result //Yes

// $array = ['blue', 'green', 'orange', 'black', 'red', '55'];
// if (in_array(55, $array)) {
//     echo "Yes";
// } else {
//     echo "No";
// }
// result // Yes while '55' != 55

// if you want to get exact answer you can use strict mode
// $array = ['blue', 'green', 'orange', 'black', 'red', '55'];
// if (in_array(55, $array, true)) {
//     echo "Yes";
// } else {
//     echo "No";
// }
// result // No (by adding 3rd argument true you may stricty get your answer)

// $array = [
//     'color' => ['blue', 'green', 'orange', 'black', 'red'],
//     'fruit' => ['apple', 'mango', 'graph', 'orange', 'banana'],
// ];
// if (in_array(['blue', 'green', 'orange', 'black', 'red'], $array)) {
//     echo "Yes";
// } else {
//     echo "No";
// }
// result // Yes also checking associative array value

// $array = [
//     ['blue', 'green', 'orange', 'black', 'red'],
//     ['apple', 'mango', 'graph', 'orange', 'banana'],
// ];
// if (in_array(['blue', 'green', 'orange', 'black', 'red'], $array)) {
//     echo "Yes";
// } else {
//     echo "No";
// }
// result // Yes | checking sub array value

// ================= search_array | search array return key/value

// $array = ['blue', 'green', 'orange', 'black', 'red', '55'];
// echo array_search('green', $array); // 1 because green is on 1 index

// $array = [
//     'color' => 'blue',
//     'fruit' => ['apple', 'mango', 'graph', 'orange', 'banana'],
// ];
// echo array_search('blue', $array); // color
