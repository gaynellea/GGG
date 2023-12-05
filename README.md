@ViewBuilder
    private func createHLine(index: Int) -> some View {
        if index == 0 {
            rectangle
                .frame(height: lineWidth)
        } else {
            VStack(spacing: 0) {
                Spacer()
                    .frame(minHeight: 0)
                rectangle
                    .frame(height: lineWidth)
            }
        }
    }
    
    private var rectangle: some View {
        Rectangle()
            .fill(.gray)
    }
}

struct GridView_Previews: PreviewProvider {
    static var previews: some View {
        GridView(xLines: 10, yLines: 10)
    }
}# GGG
