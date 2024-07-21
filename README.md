<h1 align="center">Hey 👋, I'm Mike</h1>
<h3 align="center">A Software engineer from Uganda</h3>

# mike.go

Welcome to my GitHub repository

```go
package main

import (
	"fmt"
	"time"
)

// Contact information
type Contact struct {
	Email    string
	LinkedIn string
	GitHub   string
}

type Skills struct {
	JavaScript     bool
	NextJS         bool
	ReactNative    bool
	Python         bool
	Django         bool
	Kotlin         bool
	JetpackCompose bool
}

func introduction(name string) {
	fmt.Printf("Hello, my name is %s!\n", name)
}


func showSkills(skills Skills) {
	fmt.Println("Here are my skills:")
	if skills.JavaScript {
		fmt.Println("- JavaScript")
	}
	if skills.NextJS {
		fmt.Println("- Next.js (a framework of JavaScript)")
	}
	if skills.ReactNative {
		fmt.Println("- React Native")
	}
	if skills.Python {
		fmt.Println("- Python")
	}
	if skills.Django {
		fmt.Println("- Django")
	}
	if skills.Kotlin {
		fmt.Println("- Kotlin")
	}
	if skills.JetpackCompose {
		fmt.Println("- Jetpack Compose")
	}
}

func funFacts() {
	facts := []string{
		"I love coding!",
		"I'm a coffee enthusiast.",
		"I enjoy solving complex problems.",
		"I'm a lifelong learner.",
	}

	for _, fact := range facts {
		go func(f string) {
			fmt.Println(f)
		}(fact)
	}

	time.Sleep(1 * time.Second)
}

func main() {
	name := "Mike"

	skills := Skills{
		JavaScript:     true,
		NextJS:         true,
		ReactNative:    true,
		Python:         true,
		Django:         true,
		Kotlin:         true,
		JetpackCompose: true,
	}

	introduction(name)
	showSkills(skills)
	funFacts()
}

```


<p><img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=MikeMatovu&" alt="Mike" /></p>
