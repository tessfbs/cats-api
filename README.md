# CatsAPI documentation

## /breeds

>### GET /breeds 
>
>The properties for each Breed will increase over time as more research is completed.
>Passing a Breed’s id as Query parameter breed_id on requests to the /images/search route will filter the search results to only show that Breed. 
>
>e.g. https://api.thecatapi.com/v1/images/search?breed_id=beng will return Bengal Cats
>
>Example Response:
>```javascript
>[
>    {
>        weight: {
>            imperial: "7  -  10",
>            metric: "3 - 5"
>        },
>        id: "abys",
>        name: "Abyssinian",
>        cfa_url: "http://cfa.org/Breeds/BreedsAB/Abyssinian.aspx",
>        vetstreet_url: "http://www.vetstreet.com/cats/abyssinian",
>        vcahospitals_url: "https://vcahospitals.com/know-your-pet/cat-breeds/abyssinian",
>        temperament: "Active, Energetic, Independent, Intelligent, Gentle",
>        origin: "Egypt",
>        country_codes: "EG",
>        country_code: "EG",
>        description: "The Abyssinian is easy to care for, and a joy to have in your home. They’re affectionate cats and love both people and other animals.",
>        life_span: "14 - 15",
>        indoor: 0,
>        lap: 1,
>        alt_names: "",
>        adaptability: 5,
>        affection_level: 5,
>        child_friendly: 3,
>        dog_friendly: 4,
>        energy_level: 5,
>        grooming: 1,
>        health_issues: 2,
>        intelligence: 5,
>        shedding_level: 2,
>        social_needs: 5,
>        stranger_friendly: 5,
>        vocalisation: 1,
>        experimental: 0,
>        hairless: 0,
>        natural: 1,
>        rare: 0,
>        rex: 0,
>        suppressed_tail: 0,
>        short_legs: 0,
>        wikipedia_url: "https://en.wikipedia.org/wiki/Abyssinian_(cat)",
>        hypoallergenic: 0,
>        reference_image_id: "0XYvRd7oD"
>    },
>    {
>        weight: {
>            imperial: "7 - 10",
>            metric: "3 - 5"
>        },
>        id: "aege",
>        name: "Aegean",
>        vetstreet_url: "http://www.vetstreet.com/cats/aegean-cat",
>        temperament: "Affectionate, Social, Intelligent, Playful, Active",
>        origin: "Greece",
>        country_codes: "GR",
>        country_code: "GR",
>        description: "Native to the Greek islands known as the Cyclades in the Aegean Sea, these are natural cats, meaning they developed without humans getting involved in their breeding. As a breed, Aegean Cats are rare, although they are numerous on their home islands. They are generally friendly toward people and can be excellent cats for families with children.",
>        life_span: "9 - 12",
>        indoor: 0,
>        alt_names: "",
>        adaptability: 5,
>        affection_level: 4,
>        child_friendly: 4,
>        dog_friendly: 4,
>        energy_level: 3,
>        grooming: 3,
>        health_issues: 1,
>        intelligence: 3,
>        shedding_level: 3,
>        social_needs: 4,
>        stranger_friendly: 4,
>        vocalisation: 3,
>        experimental: 0,
>        hairless: 0,
>        natural: 0,
>        rare: 0,
>        rex: 0,
>        suppressed_tail: 0,
>        short_legs: 0,
>        wikipedia_url: "https://en.wikipedia.org/wiki/Aegean_cat",
>        hypoallergenic: 0,
>        reference_image_id: "ozEvzdVM-"
>    },
>    ...
>]
>```

>### GET /breeds/search
>
>Search for a Breed by using part of it’s name as the ‘q’ query parameter.
>
>e.g ?q=sib to search for Siberian - https://api.thecatapi.com/v1/breeds/search?q=sib
>
>Example Response:
>```javascript
>[
>	{
>		weight: {
>			imperial: "8 - 16",
>		metric: "4 - 7"
>	},
>		id: "sibe",
>		name: "Siberian",
>		cfa_url: "http://cfa.org/Breeds/BreedsSthruT/Siberian.aspx",
>		vetstreet_url: "http://www.vetstreet.com/cats/siberian",
>		vcahospitals_url: "https://vcahospitals.com/know-your-pet/cat-breeds/siberian",
>		temperament: "Curious, Intelligent, Loyal, Sweet, Agile, Playful, Affectionate",
>		origin: "Russia",
>		country_codes: "RU",
>		country_code: "RU",
>		description: "The Siberians dog like temperament and affection makes the ideal lap cat and will live quite happily indoors. Very agile and powerful, the Siberian cat can easily leap and reach high places, including the tops of refrigerators and even doors. ",
>		life_span: "12 - 15",
>		indoor: 0,
>		lap: 1,
>		alt_names: "Moscow Semi-longhair, HairSiberian Forest Cat",
>		adaptability: 5,
>		affection_level: 5,
>		child_friendly: 4,
>		dog_friendly: 5,
>		energy_level: 5,
>		grooming: 2,
>		health_issues: 2,
>		intelligence: 5,
>		shedding_level: 3,
>		social_needs: 4,
>		stranger_friendly: 3,
>		vocalisation: 1,
>		experimental: 0,
>		hairless: 0,
>		natural: 1,
>		rare: 0,
>		rex: 0,
>		suppressed_tail: 0,
>		short_legs: 0,
>		wikipedia_url: "https://en.wikipedia.org/wiki/Siberian_(cat)",
>		hypoallergenic: 1,
>		reference_image_id: "3bkZAjRh1"
>	}
>]
>```

## /images

>### GET images/search
>
>Click on this to get a random Image https://api.thecatapi.com/v1/images/search
>
>Example Response:
>```javascript
>[
>    {
>        id: "dhp",
>        url: "https://cdn2.thecatapi.com/images/dhp.jpg",
>        width: 3628,
>        height: 2414
>    }
>]
>```
