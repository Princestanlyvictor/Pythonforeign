def get_suit_names():
  while True:
      try:
          num_suits = int(input("How many suits? "))
      except ValueError:
          print("Error, must be an integer!")
          continue

      if num_suits < 2:
          print("Error, must be at least 2 suits!")
          continue

      suits = []
      for i in range(num_suits):
          while True:
              suit_name = input(f"Input suit #{i + 1}: ").strip()
              if not suit_name:
                  print("Error, no input!")
                  continue

              if suit_name.lower() in suits:
                  print("Error, duplicate suit!")
                  continue

              suit_name = suit_name.title()
              if " " in suit_name:
                  print("Error, must be single word!")
                  continue

              suits.append(suit_name)
              break

      return suits


def main():
  suits = get_suit_names()
  print("Thank you. The suits are:")
  print(", ".join(suits))


if __name__ == "__main__":
  main()
