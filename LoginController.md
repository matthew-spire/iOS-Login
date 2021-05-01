```
import UIKit

class LoginController: UIViewController {
	override func viewDidLoad() {
		super.viewDidLoad()

		configureUI()
	}

	func configureUI() {
		// Hide the navigation controller
		navigationController?.navigationBar.isHidden = true
		navigationController?.navigationBar.barStyle = .black
		
		let gradient = CAGradientLayer()
		gradient.colors = [UIColor.systemPurple.cgColor, UIColor.systemBlue.cgColor]
		gradient.locations = [0, 1]
		view.layer.addSublayer(gradient)
		gradient.frame = view.frame
	}
}
```