```
func scene(...) {
	guard let scene = (scene as? UIWindowScene) else { return}
	// Instantiating the window from above
	window = UIWindow(windowScene: scene)
	window?.rootViewController = UINavigationController(rootViewController: LoginController())
	window?.makeKeyAndVisible()
}
```