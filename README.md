# ruby_warrior
The solution of  www.bloc.io/ruby-warrior .

# ruby_warrior Level 4
class Player
  def play_turn(warrior)
    if warrior.feel.empty?
      if warrior.health > 13
        warrior.walk!
      else
        if @health > warrior.health
          warrior.walk!
        else
          warrior.rest!
        end
      end
    else
      warrior.attack!
    end
    @health = warrior.health
 end
end
