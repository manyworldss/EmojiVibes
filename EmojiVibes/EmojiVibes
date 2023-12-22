//
//  ContentView.swift
//  EmojiVibes
//
//  Created by Rapheal Suber on 12/22/23.
//

import SwiftUI

enum Emoji: String, CaseIterable {
    case computer = "🖥️"
    case clown = "🤡"
    case runner = "🏃🏿‍♂️"
    case ninja = "🥷🏿"
}

struct ContentView: View {
    @State var selection = Emoji.runner
 
    var body: some View {
        NavigationView {
            VStack {
                Text(selection.rawValue)
                    .font(.system(size: 150))
                
                Picker("Select Emoji", selection: $selection) {
                    ForEach(Emoji.allCases, id:\.self) {emoji in
                        Text(emoji.rawValue)
                    }
                }
                .pickerStyle(.wheel)
            }
            .navigationTitle("Emoji Vibes!")
            .padding()
        }
    }
}

struct ContentView_Previews: PreviewProvider {
    static var previews: some View {
        ContentView()
    }
}
