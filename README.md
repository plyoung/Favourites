# Unity Favourites Panel

[![Twitter](https://img.shields.io/badge/-@pl__young-007ec6.svg?style=flat-square&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAAulBMVEUAAAAgn%2FQcovIdovMdoPAkpO0kkv8covMrqv8covMdofIdofIcovIcofEYnvMbofMdofIhpvQA%2F%2F8cofIcofIeofIbofIdofIcofIaou4dofIdofEeofIdofEdoPIeoPMdofIdofIdofIdofIdoPMeovIdoPEdofIdovMeoPIfofUdofIdofIVquogn%2B8eoPIeofIdofIcofMcovEdofMdofIdofIhpe8cn%2FEcofEeoPMbn%2FQAv%2F8dofL9CP3sAAAAPXRSTlMAGGNoIw4HkQY%2F7%2FiZvBVBxBcB4L1fJuNkHp272KhOK8H%2B2e0%2BrJT5a4kxscsMEDua%2FJA3uPZPH0hsZjAEzRmxHgAAAH9JREFUeAF1yNUSggAUANE1RBQDQxS7uzu8%2F%2F9bclEGXzgvO7NEi8UTSUhhpE1UJiti5fIFimKXgHJFVLWGI1JvuBrVBFriaXfE14VefyAhFxhKaIRn%2FHcmeIypJT8zBzWXwIKv5Up86w1qu9sfRB1N1Oks6mJfCdzuj%2BfrTZQPzs4dZmTFoZYAAAAASUVORK5CYII%3D)](https://twitter.com/pl_young)
[![Asset Store](https://img.shields.io/badge/-Asset_Store-333333.svg?style=flat-square&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAQAAAC1%2BjfqAAAA5ElEQVQoz5WRMS9DYRSGn%2B%2FmRoKFRGwWm60LE5PJbLHgH1hIdMLIH%2FADMEokOkk06cZiqJJIWK9FDK4mhOZ7LJdUlcZZn5Oc57wvdBmHXufudjx38Scad8OaeXyP0ehBJx6wYsvMiodGNTMNBQosMcsjGWfcENhjijrTzBTYFZ9sWCrWl1svD1vOGy0DJq767OUXHvMqr5%2BOOGpulePEdZs2LBkMBlO3beYLYJ8nXqSDa2zSzzC7hWnCBDWOILxZ5TYBAn9NrxOfkvk3yes2yV5v%2FhbUPpNtQXVEfd8e9f%2FK6lb3B5tlzmXUxDhbAAAAAElFTkSuQmCC)](https://assetstore.unity.com/publishers/380)
[![PayPal](https://img.shields.io/badge/-Donate-dfb317.svg?style=flat-square&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAA21BMVEX%2F%2F%2F8AAP8AQIAAJJIAIIAAYJ8AVaoAMIAAV64AJ4kAJoYAJ4UAK4UAW60AJ4YAXK0AKocAKIcAKocAKocAXa4AWqsAYK8AX7AAKYcAKocAKocAKYYAYrIAKYgAZLMAKYgAKYcAZ7UAZ7YAKYcAa7gAKYcAbLkAbLkARpgAKYcAMY4AecMAKYcAKYcAgMgAgskAGGoAGWwAGm0AHXIAHnIAIXkAInoAInsAI30AJYAAJoIAKIUAKYcALH8AMYQAPpUAP5AAXqsAXq8AbroAfcYAf8cAgMgAhMsAhcy1oBy8AAAAMHRSTlMAAQQHCAgMECYnKC4wNTtLVVlbaGt3fYGEhpOWpq2ur8DCxtjZ2trc4uTk%2Bfz9%2Fv6U8Jh7AAAAlElEQVQYGQXBy0rDQBQA0DMz1yS11MZF0UX1%2F%2F9JcKP4gFQxgdiHTDwnod%2F3cBiHEwW7e3B9u%2FyQ0QDsNwRlhb9KKlcEXc%2FpAnbjJdOggvRwJ9NiAduylmlZKtx0zoKGmlJeRcskREezyeB5ELotJcPy9EpokHiZjuMRoUVi%2BASyxFcwA8LHd1o%2FepsAWf2dz%2B9mgH8fYCsaIQYkbQAAAABJRU5ErkJggg%3D%3D)](https://www.paypal.me/plyoung)

This will add a new panel with a Tree View where you add categories and can drag-and-drop objects from the Hierarchy or Project panel into.

- The panel can be opened from menu: `Window > Favourites`.
- Use the [+] button in the Favourites panel's toolbar to add a new category.
- Use the [-] button to remove the selected category and all its items or to remove a single selected item.
- Double-click on an item to open it. For example to open a scene you have added to Favourites.
- Right-click to ping a Favourites item in the Hierarchy or Project panel.
- Drag-and-drop items to new categories or other areas of Unity. You can for example drag-and-drop a Sprite from the Favourites panel into the property of a component's Inspector (if that property accept Sprites).

#Technical Info#

The favourites system's main asset file is saved next to the editor scripts, so that would be in `\Assets\Favourites\Editor` by default.

The list of favourite scene objects however are saved in an object in the scene since assets/prefabs can't reference objects in the scene. This object is tagged as editor only so it will not end up in your final builds. You will also notice that when you close the scene the favourite scene objects will disapear from the list of favourites. It will be back when you open the scene and did not delete the category the objects was under.

![screenshot](https://user-images.githubusercontent.com/837362/34055429-d059f5ce-e1d7-11e7-8855-1b19dc2ad052.png)
