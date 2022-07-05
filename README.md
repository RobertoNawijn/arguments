def greet (name, greet = "Hello, <name>!"):
    x = greet.replace("<name>", name)
    return x

def force (mass, body = "earth"):
    gravity_list = {
        "sun" : 274,
        "jupiter" : 24.9,
        "neptune" : 11.2,
        "saturn" : 10.4,
        "earth" : 9.8,
        "uranus": 8.9,
        "venus" : 8.9,
        "mars" : 3.7,
        "mercury" : 3.7,
        "moon" : 1.6,
        "pluto" : 0.6
}
    body = gravity_list[body]
    gravity_force = body * mass
    return gravity_force
    print(force(8.9, 'venus'))

def pull (m1, m2, d):
    # pull = G * ((m1 * m2\d ** 2))
    g = 6.674 * (10**-11)
    power = (g * m1 * m2) / (d ** 2)
    return power
