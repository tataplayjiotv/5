<?php

$url = 'https://babel-in.xyz/tata/channels';
$data = [
    'X-API-Key' => 'babel-ee35e0bc5726f30817361ec0ad',    
];
$jsonData = json_encode($data);

$options = [
    'http' => [
        'header'  => [
            "Content-type: application/json",
            "User-Agent: Babel/5.0"
        ],
        'method'  => 'POST',
        'content' => $jsonData,
    ],
];

$context  = stream_context_create($options);
$response = file_get_contents($url, false, $context);

if ($response === FALSE) {
    die('Error sending request');
}

echo $response;

